
## Unity GC Cheatsheet

- Pull-requests are welcome. 
- These entries are based on Unity 5 (or newer).
- Though it's written up in Chinese, an English-translation pull request would be **espacially welcome**.
- Check out complemental pages listed below.

--------------------------

- [**Unity GC Cheatsheet**](unity-gc-cheatsheet.md)
    + [Details](unity-gc-cheatsheet-details.md)
    + [References](unity-gc-cheatsheet-references)

--------------------------

- a01. struct Foo 在栈上，但 struct Foo[] 在堆上
    + 推广： 单个的 ValueType 直接在栈上分配，但 ValueType Array 总是分配在堆上
    + This means that all arrays are always reference types which are allocated on the managed heap ([so_type01](http://stackoverflow.com/questions/1533757/is-int-a-reference-type-or-a-value-type))
- a02. GetType() 会产生 GC Alloc
    + 每个调用 20 Bytes
- a03. delegate 的创建时赋值 = 在堆上分配
    + 生成一个新的委托，例如将方法做为参数传入 ([Jare Guo](https://www.zhihu.com/question/26779558/answer/34015434))
- a04. delegate 的注册请使用 = 而不是 +=
    + 当对象被复用时， += 会导致 InvocationList 不断增长
    + 两个后果：1. 目标函数会被调用多次 2. 内存占用会随时间累积
- a05. 在针对 GC Alloc 做优化时，对象数量 > 引用关系复杂度 > 对象尺寸
- a06. 当可以使用整数句柄来代替引用时，尽量使用整数句柄 (简化引用关系)
- a07. 优化内存布局：利用“数组对 GC 而言是单一对象”这一特性

- b01. 避免频繁调用那些会分配内存的 accessors  (如 Mesh.vertices / Mesh.normals / Mesh.uvs / SkinedMeshRenderer.bones)
- b02. 避免频繁调用 Int.ToString() 及其它类型的衍生
- b03. 避免在 Update() 内使用 [GameObject.Tag](http://answers.unity3d.com/questions/1010251/gameobjecttag-without-gc-allocation.html) 和 [GameObject.Name](http://forum.unity3d.com/threads/unityengine-object-name-allocates-for-each-access.237380/)
- b04. 避免在 Update() 内 GetComponent() 
- b05. 避免在 Update() 内 GetComponentInChildren()，可自己实现无 GC 版本 (Jare Guo)
- b06. 避免在 Update() 内访问 animation 组件
- b07. 避免在 Update() 内 FindObjectsOfType()
- b08. 避免在 Update() 里赋值给栈上的数组，会触发堆内的反复分配
- b09. 避免频繁使用 Mathf.Max 等函数的数组版（只要不是两个元素的，都会调到数组版） (robert01) 
- b10. (b09 推广)：所有具有 params 修饰的函数都应避免频繁使用（以避免临时数组的分配）

- c01. 在不需要时避免使用 GUILayout - OnGUI 时把 useGUILayout 关掉
- c02. 避免使用 foreach （除非遍历数组，或直接用 VS 预编译好的 dll）（Unity 5.5 已修复此问题，见这里）
- c03. 避免使用枚举或 struct 做 Key 进行字典查找 (除非使用定制的 comparer)
- c04. 避免使用字符串版本的 Invoke 和 StartCoroutine
- c05. 避免在产品中调用 Debug.Log (生成堆栈字符串)
- c06. 避免在产品中使用 Linq
- c07. 在可能的情况下复用成员变量而不是不断分配新对象
- c08. 初始化 List<> 时指定合理的 Capacity
- c09. 使用 StringBuilder 而不是使用 “+” 或 String.Concat() 拼接字符串
- c10. 在使用协程 yield 时尽量复用 WaitXXX 对象 (使用 Yielders.cs ) 而不是每次分配
- c11. 确保 struct 实现了 IEquatable<T> (robert02)
- c12. 确保 struct 实现了 Equals() 和 GetHashCode() (robert02)

--------------------------






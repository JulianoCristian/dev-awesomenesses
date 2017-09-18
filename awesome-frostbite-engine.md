
# Awesome-Frostbite-Engine

- This page contains a comprehensive collection of Frostbite Engine Resources during 2007-2017.
- These resources are available on [dice.se](http://www.dice.se/), [ea.com/frostbite](https://www.ea.com/frostbite) and [slideshare.net](https://www.slideshare.net/).
- For a brief history & list of games, check out [Frostbite on wikipedia][wikipedia].

[wikipedia]: https://en.wikipedia.org/wiki/Frostbite_(game_engine)

## "Move to One Engine"

EA is moving its games, including Mass Effect and FIFA, [onto a single graphics engine](http://www.techradar.com/news/gaming/from-battlefield-to-fifa-here-s-what-ea-s-frostbite-revolution-means-for-you-1323291). Frostbite has evolved to become the cornerstone of these titles:

- `FIFA` (FIFA 17/18)
- `Mass Effect` (Mass Effect: Andromeda)
- `Battlefield` (Battlefield 1 - 2016)  
- `Need for Speed` (NEED FOR SPEED 2017: PAYING IT BACK)
- `Mirror's Edge` (Mirror's Edge Catalyst - 2016)
- `Star Wars` (Star Wars Battlefront) 
- `Dragon Age` (Dragon Age: Origins)

## Resources

### Engine & Pipeline 

Year | Conf       | Title | Note
---- | ---------- | ----- | ----
2007 | gdc2007    | [Frostbite Rendering Architecture][render-arc] | 
2008 | gh2008     | [The Intersection of Game Engines and GPUs – Current & Future][intersection-game-engines-gpus] | 
2009 | siggraph09 | [Parallel Graphics in Frostbite – Current & Future][parallel-graphics] | 
2009 | intel2009  | [Parallel Futures of a Game Engine][parallel-engine-1] | 
2010 | stockholm  | [Parallel Futures of a Game Engine v2.0][parallel-engine-2] | 
2011 | nv-lan-6   | [Shiny PC Graphics in Battlefield 3][shiny] ([on SlideShare][shiny-2]) | 
2013 | stockholm  | [Scaling the Pipeline][scaling]| `Asset Pipeline`
2015 | siggraph15 | [The Rendering Pipeline - Challenges & Next Steps][pipeline]| 
2016 | gdc2016    | [Optimize the graphics pipeline with compute][opt-compute]| 
2017 | gdc2017    | [FRAMEGRAPH: Extensible Rendering Architecture in Frostbite][framegraph]| 

[render-arc]: http://www.dice.se/news/frostbite-rendering-architecture-real-time-procedural-shading-texturing-techniques/
[intersection-game-engines-gpus]: http://www.dice.se/news/intersection-game-engines-gpus-current-future/
[parallel-graphics]: http://www.dice.se/news/parallel-graphics-frostbite-current-future/
[parallel-engine-1]: http://www.dice.se/news/parallel-futures-game-engine-2/
[parallel-engine-2]: http://www.dice.se/news/parallel-futures-game-engine-v2-0/
[shiny]: http://www.dice.se/news/shiny-pc-graphics-battlefield-3/
[shiny-2]: https://www.slideshare.net/DICEStudio/shiny-pc-graphics-in-battlefield-3?from_action=save
[scaling]: http://www.dice.se/news/scaling-pipeline/
[pipeline]: https://www.slideshare.net/repii/the-rendering-pipeline-challenges-next-steps
[opt-compute]: https://www.ea.com/frostbite/news/optimizing-the-graphics-pipeline-with-compute
[framegraph]: https://www.ea.com/frostbite/news/framegraph-extensible-rendering-architecture-in-frostbite

### GDC 2011 & 2012 - Frostbite 2 & Battlefield 3/4

- GDC11 - `DX11` [DirectX 11 Rendering in Battlefield 3](http://www.dice.se/news/directx-11-rendering-battlefield-3/)
- GDC11 - `Lighting` [Lighting you up in Battlefield 3](http://www.dice.se/news/lighting-battlefield-3/)
- GDC11 - `Culling` [Culling the Battlefield Data Oriented Design in Practice](http://www.dice.se/news/culling-battlefield-data-oriented-design-practice/)
- GDC11 - `Deferred-Shading` [SPU-based Deferred Shading in Battlefield 3](http://www.dice.se/news/spu-based-deferred-shading-battlefield-3-playstation-3/)
- GDC11 - `SSS` [Approximating Translucency for a Fast, Cheap and Convincing Subsurface Scattering Look](http://www.dice.se/news/approximating-translucency-fast-cheap-convincing-subsurface-scattering-look/)
- GDC12 - `Animation` [Modular Rigging in Battlefield 3](http://www.dice.se/news/modular-rigging-battlefield-3/)
- GDC12 - `Terrain` [Terrain in Battlefield 3: A Modern, Complete and Scalable System](http://www.dice.se/news/terrain-battlefield-3-modern-complete-scalable-system/)
- GDC12 - `SSAO` [Stable SSAO in Battlefield 3 with Selective Temporal Filtering](http://www.dice.se/news/stable-ssao-battlefield-3-selective-temporal-filtering/)
- [(2013) `Mantle` #APU13 Mantle for Developers](https://www.ea.com/frostbite/news/mantle-for-developers)
- [(2013) `Mantle` #GPU14 Battlefield 4 + Frostbite + Mantle](http://www.dice.se/news/battlefield-4-frostbite-mantle/)
- [(2014) `Mantle` #gdc2014 Rendering Battlefield 4 with Mantle](http://www.dice.se/news/rendering-battlefield-4-mantle/)

### Rendering & Visual Effects

- [(2007) #siggraph07 Terrain Rendering in Frostbite using Procedural Shader Splatting](http://www.dice.se/news/terrain-rendering-frostbite-using-procedural-shader-splatting/)
- [(2007) Real-Time Hair Simulation and Visualisation for Games](http://www.dice.se/news/real-time-hair-simulation-visualisation-games/)
- [(2008) Procedural deformation and destruction in real-time](http://www.dice.se/news/procedural-deformation-destruction-real-time/)
- [(2009) Interactive Real Time Cloth Simulation with Adaptive Level of Detail](http://www.dice.se/news/interactive-real-time-cloth-simulation-adaptive-level-detail/)
- [(2009) Advanced Real-time Post-Processing using GPGPU techniques](http://www.dice.se/news/advanced-real-time-post-processing-using-gpgpu-techniques/)
- [(2009) Lighting and materials for real-time game engines](http://www.dice.se/news/lighting-materials-real-time-game-engines/)
- [(2009) #gdc09 The Unique Lighting in Mirror’s Edge](http://www.dice.se/news/unique-lighting-mirrors-edge/)
- [(2009) #gdc09 Single-pass Stable Cascaded Bounding Box Shadow Maps and Geometry-shader based Decal Generation](http://www.dice.se/news/shadows-decals-d3d10-techniques-frostbite/)
- [(2010) #siggraph2010 A Real-time Radiosity Architecture](http://www.dice.se/news/real-time-radiosity-architecture/)
- [(2010) #siggraph2010 Bending the Graphics Pipeline](http://www.dice.se/news/bending-graphics-pipeline/)
- [(2010) #siggraph2010 5 Major Challenges in Interactive Rendering](http://www.dice.se/news/5-major-challenges-interactive-rendering/)
- [(2011) #siggraph2011 More Performance - Five Rendering Ideas from Battlefield 3 and Need For Speed The Run](http://www.dice.se/news/performance-five-rendering-ideas-battlefield-3-need-speed-run/)
- [(2012) #thesis Real-time Interactive Water Waves](http://www.dice.se/news/realtime-interactive-water-waves/)
- [(2012) 5 major challenges in real-time rendering](http://www.dice.se/news/5-major-challenges-real-time-rendering/)
- [(2012) Data Oriented Interactive Water - An Interactive Water Simulation For PlayStation 3](http://www.dice.se/news/data-oriented-interactive-water/)
- [(2012) Adaptive Hardware-accelerated Terrain Tessellation](http://www.dice.se/news/adaptive-hardware-accelerated-terrain-tessellation/)
- [(2014) #siggraph2014 Moving Frostbite to PBR](https://www.ea.com/frostbite/news/moving-frostbite-to-pb)
- [(2015) #siggraph2015 Frostbite on mobile](https://www.ea.com/frostbite/news/frostbite-on-mobile)
- [(2015) #siggraph2015 Stochastic Screen-Space Reflections](https://www.ea.com/frostbite/news/stochastic-screen-space-reflections)
- [(2015) #siggraph2015 Physically Based and Unified Volumetric Rendering in Frostbite](https://www.ea.com/frostbite/news/physically-based-unified-volumetric-rendering-in-frostbite)
- [(2016) #gdc2016 Lighting the city of glass - Rendering ‘Mirror’s Edge Catalyst’](https://www.ea.com/frostbite/news/lighting-the-city-of-glass)
- [(2016) #gdc2016 Photogrammetry and Star Wars Battlefront - Frostbite](https://www.ea.com/frostbite/news/photogrammetry-and-star-wars-battlefront)
- [(2016) #siggraph2016 Physically Based Sky, Atmosphere & Cloud Rendering](https://www.ea.com/frostbite/news/physically-based-sky-atmosphere-and-cloud-rendering)
- [(2017) #gdc2017 4K Checkerboard in Battlefield 1 and Mass Effect Andromeda](https://www.ea.com/frostbite/news/4k-checkerboard-in-battlefield-1-and-mass-effect-andromeda)
- [(2017) #gdc2017 High Dynamic Range color grading and display in Frostbite](https://www.ea.com/frostbite/news/high-dynamic-range-color-grading-and-display-in-frostbite)

### General Programming

- [(2010) DICE Coders Day 2010 - Scope Stack Allocation](http://www.dice.se/news/scope-stack-allocation/)
- [(2010) DICE Coders Day 2010 - Introduction to Data Oriented Design](http://www.dice.se/news/introduction-data-oriented-design/)
- [(2010) DICE Coders Day 2010 - A Step Towards Data Orientation](http://www.dice.se/news/step-towards-data-orientation/)
- [(2011) Executable Bloat – How it happens and how we can fight it](http://www.dice.se/news/executable-bloat-happens-can-fight/)
- [(2011) Battlelog – Building scalable web sites with tight game integration](http://www.dice.se/news/battlelog-building-scalable-web-sites-tight-game-integration/)

### Gameplay & Input

- [(2009) #gdc2009 Creating First Person Movement for Mirror’s Edge](http://www.dice.se/news/creating-first-person-movement-mirrors-edge/)
- [(2010) #gdc2010 Mirrors Edge Level Design Challenges & Solutions](http://www.dice.se/news/mirrors-edge-level-design-challenges-solutions/)
- [(2012) #thesis Motion Controllers for Game Consoles (PlayStation Move and Microsoft’s Kinect)](http://www.dice.se/news/motion-controllers-game-consoles/)

### Papers & Detailed Reports

- [(2014) Per-face parameterization for Texture Mapping of Geometry in Real-Time](https://www.ea.com/frostbite/news/per-face-parameterization-for-texture-mapping-of-geometry-in-real-time)
- [(2015) Surface Data On Dynamic Topologies](http://www.dice.se/news/master-thesis-surface-data-dynamic-topologies/)
- [(2017) #i3d2017 Tiled light trees](https://www.ea.com/frostbite/news/tiled-light-trees) ([Paper](http://yuriyodonnell.com/publications/TiledLightTrees-preprint.pdf))
- [(2017) Matching of geometrically and topologically changing meshes](https://www.ea.com/frostbite/news/matching-of-geometrically-and-topologically-changing-meshes)


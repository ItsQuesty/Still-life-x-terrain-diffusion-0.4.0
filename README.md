# Still-life-x-terrain-diffusion-0.4.0
Still Life × Terrain Diffusion
A Fabric 1.21.1 compatibility mod that bridges Still Life onto Terrain Diffusion’s AI-generated terrain.
Terrain Diffusion replaces Minecraft’s overworld generation with an ONNX diffusion model and a limited vanilla biome palette. Still Life normally uses its own large multi-noise biome set on Lithosphere terrain. This mod connects the two systems so Terrain Diffusion worlds can use Still Life’s biomes, surfaces, features, vegetation, mob spawning, colors, and cave biomes across every TD world scale.
It also adds terrain-derived upland freshwater generation, allowing streams and basin lakes to appear above sea level where Still Life river and wetland biomes need actual water to function.
What it does
Adds the sltd:climate_bridge biome source.
Overrides Terrain Diffusion’s overworld preset to use Still Life biome selection.
Converts Terrain Diffusion physical outputs — elevation, slope, temperature, precipitation — into Minecraft climate parameters.
Runs Still Life’s own multi-noise biome search at runtime.
Supports all Still Life biomes without bundling Still Life data.
Applies Still Life surface rules to Terrain Diffusion terrain.
Rescales alpine/snow height anchors for Terrain Diffusion world scale.
Generates upland freshwater streams and basin lakes on TD terrain.
Configures Distant Horizons for correct distant terrain generation.
Projects Still Life biomes into Fabric common c: biome tags for better mod compatibility.
Requirements
Minecraft 1.21.1
Fabric Loader 0.18.1+
Fabric API
Java 21+
Terrain Diffusion 2.x
Still Life
Lithosphere
Lithosphere must remain installed because Still Life references its data, but Terrain Diffusion still provides the actual terrain density.
Compatibility
Supported/tested in principle:
Distant Horizons
Farmer’s Delight Refabricated
Serene Seasons + GlitchCore
Sodium
Lithium
FerriteCore
ImmediatelyFast
Iris
BadOptimizations
Not compatible for this Fabric release:
Project Atmosphere 1.21.1, because its available build is NeoForge-only.
Status
Version 0.4.0 supports Still Life biomes, surfaces, features, mob spawning, colors, scale-aware alpine/snow behavior, upland freshwater, Distant Horizons configuration, and common biome tags.
The main remaining work is climate calibration: tuning the physical-to-Minecraft climate mapping against a normal Lithosphere + Still Life world for a closer biome distribution match.

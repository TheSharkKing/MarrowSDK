# Changelog
All notable changes to this package will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [1.2.0]

### Added

- Fixtures: DataCard representing Spawnables pinned to the world
- Backlot Fixtures: Buttons, Switch, Lever, Slider, Airlock Door
- AssetWarehouse Drag And Drop: Drag and Drop Spawnables and Fixtures straight from the warehouse into your scene!
- Circuits: Wiring needed to connect fixtures together
- Circuit Nodes: Add, Multiply, Remap, Value, FlipFlip, Xor
- EntityPose: DataCard for posing entities, use these with Circuit Fixtures to set their initial state

### Known Issues

- Custom Spawnables unsupported


## [1.1.0]

### Added

- ImpactProperties & SurfaceDataCard: Adds physical properties to the environment
- ZoneAggro: ZoneLinkItem that alerts enemies of the player
- SpawnForce: Adds initial force to a spawnable, let those crablets fly!
- SurfaceDataPainter: Tooling to help visualize and apply SurfaceDataCards to ImpactProperties
- Experimental Level Utilities window, use this to automatically create Reflection/Light Probes and Volumetrics

### Changed

- Better Pallet Inspector, easier to access Create Crate and Create DataCard buttons

### Fixed

- Fixed skybox rendering black
- Fixed the Project Layers to use the correct Marrow Layers
- Fixed CrateSpawner Title not changing properly

### Known Issues

- Custom Spawnables unsupported


## [0.6.0]

### Added

- Zone, ZoneLink
- ZoneItems: ZoneEvents, ZoneLoadLevel
- ZoneLinkItems: ZoneAmbience, ZoneMusic, ZoneChunkLoader
- ZoneCuller, SceneChunk
- DataCard
- DataCards: BoneTag and MonoDisc
- Pallet Dependencies
- PreviewMesh and MonoDisc loading in the editor for previewing content from built external pallets
- CrateSpawner (Replacing SpawnableCratePlacer)
- Zone Creation/Linking Overlay (Spacebar in sceneview to enable)
- Added Normal Map Encoding and Lightmap Encoding rules to Marrow Project Validation
- Added URP Quality Settings and Shader Import rules to Marrow Project Validation
- AudioReverbData, used in ZoneAmbience (use these instead of Unity's Reverb Zones)
- AssetWarehouse Reload button, hit this bad boy anytime you think the AssetWarehouse might be out of sync!
- Getting Started Window

### Changed

- Updated to Unity Version 2021.3.16f1
- Marrow Project Validation fully automatic, will run on its own now, no longer a manual step
- New smoother workflow from package installation to creating Pallets and LevelCrates
- Updated URP/Core dependencies
- Smoother package installation/updating using Scoped Registries (Remove all current SDK/URP packages in the package manager for best results)
- All SDK related components are now sorted in the Add Component Menu under MarrowSDK
- External Pallets are now loaded into memory using the Add Pallet Dependency button on the Pallet (Delete any External Pallets that were previously imported into your project)
- Addressables re-work to load bundles more dynamically
- Smoother AssetWarehouse window User Experience

### Fixed

- AssetWarehouse now recovers after exiting Playmode
- Addressables breaking after building
- Proper AssetWarehouse asynchronus reloading
- Various issues with Marrow Project Validation
- Platform now restores after you do a build for a different platform

### Known Issues

- Skybox will render as black
- Layers may appear to be missing (The layers will still work properly, needs to be added to Marrow Project Validation)
- Custom Spawnables unsupported
- CrateSpawner Title not changing properly

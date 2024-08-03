## Properties

| Prop Name | Value | Description |
| --------------------- | ------ | ------------------- |
| configMode | boolean | Enables/disables display of config mode (plugin settings) UI |
| configMetadata | **[IPluginConfig](/Documentation/Interfaces/IPluginConfig.md)** | Info Later |
| outputFolders | { id:string; path:string }[] | id: idk <br/> path: folder path? |
| guidToAsset | { [guid:string]: { metadata:**[ILibraryAssetMetadata](/Documentation/Interfaces/ILibraryAssetMetadata.md)**, binaryData?:Uint8Array, filename?:string } } | |
| spriteEntityAssets | **[ISpriteEntityAssetMetadata[]](/Documentation/Interfaces/ISpriteEntityAssetMetadata.md)** | |
| imageAssets | **[IImageAssetMetadata[]](/Documentation/Interfaces/IImageAssetMetadata.md)** | |
| audioAssets | **[IAudioAssetMetadata[]](/Documentation/Interfaces/IAudioAssetMetadata.md)** | |
| scriptAssets | **[IScriptAssetMetadata[]](/Documentation/Interfaces/IScriptAssetMetadata.md)** | |
| paletteCollectionAssets | **[IPaletteCollectionAssetMetadata[]](/Documentation/Interfaces/IPaletteCollectionAssetMetadata.md)** | |
| binaryAssets | **[IBinaryAssetMetadata[]](/Documentation/Interfaces/IBinaryAssetMetadata.md)** | |
| nineSliceAssets | **[INineSliceAssetMetadata[]](/Documentation/Interfaces/INineSliceAssetMetadata.md)** | |
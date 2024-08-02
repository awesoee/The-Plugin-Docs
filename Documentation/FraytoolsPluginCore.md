## Functions

| Function Name | Description |
| --------------------- | ------------------- |
| log(level:string, ...args):void |    Function for sending log messages back to the parent. <br/> <br/> **@param level** Log level (log, info, warn, error, or debug) <br/> **@param args** Arguments to pass to the log function.|
| configMetadataSync(configMetadata:IPluginConfig) | Informs the parent window to sync and persist the specified config metadata. <br/> <br/> **@param pluginType** The type of plugin. <br/> **@param configMetadata** The metadata to sync.|
| assetMetadataSync(assetMetadata: ILibraryAssetMetadata) | Informs the parent window to sync and persist the specified asset metadata. <br/> <br/>  |

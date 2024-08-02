## Functions

| Function Name | Description |
| --------------------- | --------------------------------- |
| log(level: string, ...args):void |    Function for sending log messages back to the parent. <br/> <br/> **@param level** Log level (log, info, warn, error, or debug) <br/> **@param args** Arguments to pass to the log function. |
| configMetadataSync(configMetadata: [IPluginConfig](/Documentation/Interfaces/IPluginConfig.md)) | Informs the parent window to sync and persist the specified config metadata. <br/> <br/> **@param pluginType** The type of plugin. <br/> **@param configMetadata** The metadata to sync. |
| assetMetadataSync(assetMetadata: [ILibraryAssetMetadata](/Documentation/Interfaces/ILibraryAssetMetadata.md)) | Informs the parent window to sync and persist the specified asset metadata. <br/> <br/> **@param pluginType** The type of plugin. <br/> **@param configMetadata** The metadata to sync. |
| sendready() | Informs the parent window that the plugin is mounted. |
| sendTypeDefinitions(typeFilesData: [ITypeDefinitionFile[]](/Documentation/Interfaces/ITypeDefinitionFile.md)) | |
| sendMetadataDefinitions(metadataDefinitions: [IMetadataDefinition[]](/Documentation/MetadataPlugin/IMetadataDefinition.md)) | |
| sendAssetMetadataMigrations(assetMetadata: [ILibraryAssetMetadata](/Documentation/Interfaces/ILibraryAssetMetadata.md)) | |
| sendPublishStart() | |
| sendPublishEnd(files: PublishPluginMessageDataFilesMap) | |
| sendPublishError(message: string) | |

## Arrow Functions

| Function Name | Description |
| ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| setupHandler:(props: any) => void | Assign a callback to this field which will be run after the plugin receives a 'loadPlugin' command from the parent. |
| propsReceivedHandler:(props: any) => void | Assign a callback to this field to handle pluginPropsReceived events. |
| migrationHandler: (configMetadata: any) => void | Assign a callback to this field to run against the plugin configMetadata before the setup process begins. This can be used to migrate the data based on the plugin's current version. |
| typeDefinitionRequestHandler:() => void | Assign a callback to this field to handle a request for types data from the parent plugin. |
| metadataDefinitionRequestHandler:() => void | Assign a callback to this field to handle a request for metadata definition data from the parent plugin. |
| assetMetadataMigrationRequestHandler:() => void | Assign a callback to this field to handle a request for metadata migration data from the parent plugin. |
| forcePublishRequestHandler:() => void | Assign a callback to this field to handle a request to force start a publish. |

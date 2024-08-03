**This class is an extension of [IPublishPluginProps](/Documentation/PublishPlugin/BasePublishPlugin/IPublishPluginProps.md) and [IPublishPluginState.](/Documentation/PublishPlugin/BasePublishPlugin/IPublishPluginState.md)**

<br/>

_**Base class for React-powered publish plugins.**_
  
_**Note that this same setup structure could be used in a Vanilla JS component as well. The main requirements are as follows:**_

1) Assign a callback to FrayToolsCore.propsReceivedHandler to handle new props being passed to the plugin from the parent window.

3) Assign a callback to FrayToolsCore.forcePublishHandler to handle when the parent window requests a forced publish.

5) Assign a callback to FrayToolsCore.setupHandler that render a UI using the props passed to the function (check "props.configMode" to determine what view to render)
6) Use FrayToolsPluginCore.sendReady() after the above steps are completed and plugin DOM is ready.
To inform the parent window that it's time to publish, use FrayToolsPluginCore.sendPublish(). This will cause the parent UI to lock. When the publish logic is completed, send use FrayToolsPluginCore.sendPublishEnd(publishData) to pass the data back to FrayTools to export. To sync plugin configuration data that should persist between sessions to the filesystem, use FrayToolsPluginCore.configMetadataSync('PublishPlugin', yourConfigMetadata).**_

<br/>

| Function Name | Description |
| ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| componentDidMount() | Ill add info once i learn more about this |
| componentWillUnmount() | |
| onMetadataDefinitionRequest() | Not implemented. |
| onAssetMetadataMigrationRequest() | Not implemented. |
| onPropsUpdated(props:[IMetadataDefinitionPluginProps](/Documentation/MetadataPlugin/BaseMetadataDefinitionPlugin/IMetadataDefinitionPluginProps.md)) | Override this with custom behavior |

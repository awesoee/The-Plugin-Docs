**This class is an extension of [IMetadataDefinitionPluginProps](/Documentation/MetadataPlugin/BaseMetadataDefinitionPlugin/IMetadataDefinitionPluginProps.md) and [IMetadataDefinitionPluginState.](/Documentation/MetadataPlugin/BaseMetadataDefinitionPlugin/IMetadataDefinitionPluginState.md)**

<br/>

_**Base class for React-powered metdata definition plugins.**_

_**Note that this same setup structure could be used in a Vanilla JS component as well. The main requirements are as follows:**_ <br/>

_**1) Assign a callback to FrayToolsCore.propsReceivedHandler to handle new props being passed to the plugin from the parent window.**_

_**2) Assign a callback to FrayToolsCore.setupHandler that render a UI using the props passed to the function (check "props.configMode" to determine what view to render)**_

_**3) Use FrayToolsPluginCore.sendReady() after the above steps are completed and plugin DOM is ready.** <br/>_

_**To sync plugin configuration data that should persist between sessions to the filesystem, use FrayToolsPluginCore.configMetadataSync('MetadataDefinitionPlugin', yourConfigMetadata).**_

<br/>

| Function Name | Description |
| ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| componentDidMount() | Sets up **propsReceivedHandler**, **metadataDefinitionRequestHandler**, and **assetMetadataMigrationRequestHandler**. Once done, calls the **sendReady()** function to tell the window that the plugin has been mounted. |
| componentWillUnmount() | Sets **propsReceivedHandler**, **metadataDefinitionRequestHandler**, and **assetMetadataMigrationRequestHandler** to `null`. |
| onMetadataDefinitionRequest() | ![image](https://github.com/user-attachments/assets/e8febf30-238b-452b-a83b-754149f8b64f) |
| onAssetMetadataMigrationRequest() | ![image](https://github.com/user-attachments/assets/559d8e8e-08e1-4f8e-84ad-529febcb4635) |
| onPropsUpdated(props:**[IMetadataDefinitionPluginProps](/Documentation/MetadataPlugin/BaseMetadataDefinitionPlugin/IMetadataDefinitionPluginProps.md)**) | Override this with custom behavior. |

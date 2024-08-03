**This class is an extension of [IScriptAssetPluginProps](/Documentation/ScriptPlugin/BaseScriptAssetPlugin/IScriptAssetPluginProps.md) and [IScriptAssetPluginState.](/Documentation/ScriptPlugin/BaseScriptAssetPlugin/IScriptAssetPluginState.md)**

<br/>

_**Base class for React-powered script types plugins.**_

_**Note that this same setup structure could be used in a Vanilla JS component as well. The main requirements are as follows:**_ <br/>

_**1) Assign a callback to FrayToolsCore.propsReceivedHandler to handle new props being passed to the plugin from the parent window.**_

_**2) Assign a callback to FrayToolsCore.setupHandler that render a UI using the props passed to the function (check "props.configMode" to determine what view to render)**_

_**3) Use FrayToolsPluginCore.sendReady() after the above steps are completed and plugin DOM is ready.** <br/>_

_**To sync plugin configuration data that should persist between sessions to the filesystem, use FrayToolsPluginCore.configMetadataSync('ScriptAssetPlugin', yourConfigMetadata).**_

<br/>

| Function Name | Description |
| ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| componentDidMount() | Sets up **propsReceivedHandler**, then calls the **sendReady()** function to tell the window that the plugin has been mounted. |
| componentWillUnmount() | Sets **propsReceivedHandler** to `null`. |
| onPropsUpdated(props:**[IScriptAssetPluginProps](/Documentation/ScriptPlugin/BaseScriptAssetPlugin/IScriptAssetPluginProps.md)**) | Override this with custom behavior. |
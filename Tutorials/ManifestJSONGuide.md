# Before You Begin

**Before you learn how to customize stuff, let me introduce you to a _really_ helpful command:** `npm run dev`.
![image](https://github.com/user-attachments/assets/d4255069-1341-47f2-903c-f9993502a79e)

Run this in your terminal to instantly apply changes made in VS Code to your FrayTools plugin! <br/>
It's really convenient and will save you *a lot* of time.


## Updating Your Manifest.JSON / Renaming Your Plugin

For these demonstrations, I'll be using the [example metadata plugin.](https://github.com/awesoee/ts-metadata-plugin-example) The steps below work for any plugin type.

### In VS Code, navigate to static/manifest.json.
![image](https://github.com/user-attachments/assets/414802d5-4e4c-43ef-b910-2db9cb039fb0) <br/>

You can learn more about what each property does by [clicking here.](/Documentation/Interfaces/IManifestJSON.md)

### Change the `id` and `name`.

![image](https://github.com/user-attachments/assets/499ecde9-83c1-4fc3-a965-13970e6aadb4) <br/>

You can also change the `description` if you want. <br/>
**Do not change the `type` property.**

### Right-click your manifest.json and click Save.

![image](https://github.com/user-attachments/assets/eb94efe5-9153-4b95-9cb5-cbec36d98c8f)

### Now, navigate to webpack.config.js.

![image](https://github.com/user-attachments/assets/b567e58f-905b-45b9-bdb4-5e46329f805c)

### Change the value of pluginName.

![image](https://github.com/user-attachments/assets/b42f05d0-887a-455e-9f99-923a7bdd275f)


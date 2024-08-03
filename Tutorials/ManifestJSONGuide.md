# Before You Begin

**Before you learn how to customize stuff, let me introduce you to a _really_ helpful command:** `npm run dev`.
![image](https://github.com/user-attachments/assets/d4255069-1341-47f2-903c-f9993502a79e)

Run this in your terminal to instantly apply changes made in VS Code to your FrayTools plugin! <br/>
It's really convenient and will save you *a lot* of time.


## Updating Your Manifest.JSON / Renaming Your Plugin

For these demonstrations, I'll be using the [example metadata plugin.](https://github.com/awesoee/ts-metadata-plugin-example) The steps below work for any plugin type.

### In VS Code, navigate to static/manifest.json.
![image](https://github.com/user-attachments/assets/414802d5-4e4c-43ef-b910-2db9cb039fb0) <br/>

You can learn more about each property by [clicking here.](/Documentation/Interfaces/IManifestJSON.md)

### Change the `id` and `name`.

![image](https://github.com/user-attachments/assets/499ecde9-83c1-4fc3-a965-13970e6aadb4) <br/>

You can also change the `description` if you want. <br/>
**Do not change the `type` property.**

### Right-click your manifest.json and click Save.

![image](https://github.com/user-attachments/assets/eb94efe5-9153-4b95-9cb5-cbec36d98c8f)

### Open types.ts and update the pluginMetadata with your new `id`.

Click Save when you're done.

![image](https://github.com/user-attachments/assets/efae6a7c-ad7c-4ab8-b98a-9a5f8dbae862)

### Now, navigate to webpack.config.js.

![image](https://github.com/user-attachments/assets/b567e58f-905b-45b9-bdb4-5e46329f805c)

### Change the value of pluginName.

![image](https://github.com/user-attachments/assets/b42f05d0-887a-455e-9f99-923a7bdd275f)

### Click Save.

You should be getting used to saving by now.

![image](https://github.com/user-attachments/assets/fa1778a0-c6e2-4e4a-81a9-9da4c6f56dc1)

### Open main.tsx.

![image](https://github.com/user-attachments/assets/aee9ac5f-a42c-49de-bd75-e459f1853c0d)

### Change the className of the app container.

![image](https://github.com/user-attachments/assets/e9406a70-4155-44db-96f7-605daeecd4a7)

### Now, open up MyMetadataDefinitionPlugin.tsx and do the same thing there.

It should be on line 39. **Do not remove the period to the left.**

![image](https://github.com/user-attachments/assets/75667c7d-1196-4f72-b981-86ce4a6b8eb8)

### Save everything.

If you close and reopen the Plugin Manager, you should see your changes apply instantly if you ran `npm run dev`.

![image](https://github.com/user-attachments/assets/a1bcfe9c-b989-496a-af47-d8c05e36769d)


### Next Guide: Customizing Your Config Menu

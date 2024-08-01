# Fundamental Knowledge

**Plugins are typically written in TypeScript and utilize the React and React-DOM libraries.** You really don't need to be an expert in any of these in order to make plugins (typescript has a *very* similar syntax to hscript, the language used to make fraytools characters) but the more knowledge the better.

Here are a couple resources to learn more:
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [React Tutorial](https://react.dev/learn)
- [React References](https://react.dev/reference/react#)

There are four plugin types natively supported by Fraytools:

**Metadata Plugins** - Add custom buttons and fields to the Properties panel <br/>
**Publish Plugins** - Create your own UI for exporting/publishing Fraytools projects <br/>
**Types Plugins** - Create custom type definitions <br/>
**Script Asset Plugins** - Add additional pages to the script editor <br/>

# Setting Up

- You will need an IDE (Integrated Development Environment, basically code editor) to create plugins. I reccommend [Visual Studio Code.](https://code.visualstudio.com/)
- Install the latest LTS version of [Node.js.](https://nodejs.org/en/)
- Download one of my [upgraded example plugins.](https://github.com/awesoee/ts-types-plugin-example/tree/main)

<br/>

### 1. Open Visual Studio Code and click Open Folder.

  ![image](https://github.com/user-attachments/assets/06d5a406-71b9-4585-8ac2-1152dc9c4666)

<br/>

### 2. Find your example plugin and click Select Folder.
![image](https://github.com/user-attachments/assets/0ef470f2-e41b-4174-9bd2-2f45122bcf5b)

<br/>

### 3. Click the Terminal tab on the top bar, then click New Terminal.
![image](https://github.com/user-attachments/assets/99754640-b636-48c4-b735-af0bf5e9a7d9)

<br/>

### 4. In the terminal, run the command `npm install`.
![image](https://github.com/user-attachments/assets/931b0788-6b48-451d-822c-33e27e467418)

If there appears to be vulnerablilities, run the command `npm audit fix`.
![image](https://github.com/user-attachments/assets/49a6c1a3-424f-41a9-a7fe-81f5eb95906a)





![image](https://user-images.githubusercontent.com/84402719/214473123-5a483e30-6815-4e75-8e4a-903ba83a3dde.png)

### Creater 
[Piyush Yadav](https://heypiyush.vercel.app/)


A colorful mix of [Ayu](https://marketplace.visualstudio.com/items?itemName=teabyii.ayu), Lucy and [Andromeda](https://marketplace.visualstudio.com/items?itemName=EliverLara.andromeda) themes.

---

## Example

### React

![image](https://user-images.githubusercontent.com/84402719/214473248-27e4905b-cf43-4654-9f3f-a1f232f4028d.png)


### More examples

<details>
<summary>C++</summary>

![image](https://user-images.githubusercontent.com/84402719/214473562-1ee877b4-72b9-454f-821a-86317a238708.png)
</details>

<details>
<summary>CSS</summary>

![image](https://user-images.githubusercontent.com/84402719/214473722-5269685d-33b5-4261-b7a0-f3a2a9cf377d.png)

</details>

<details>
<summary>Typescript</summary>

![image](https://user-images.githubusercontent.com/84402719/214473958-06a6c548-d69d-48f8-be9d-4aa280899a27.png)

</details>

<details>
<summary>Python</summary>

![image](https://user-images.githubusercontent.com/84402719/214474238-f36bd09a-c069-41a7-8d2f-d6a503aa3c89.png)

</details>


## Install

### Via the VS Code Marketplace

- Go to the [marketplace](https://marketplace.visualstudio.com/items?itemName=piyush-yadav-india.darking-horse).
- Click on the **Install** button.
- Wait for the extension to be installed.
- Select a variant: Dark (default). Alternatively, you can also use VS Code's `autoDetectColorScheme` to enable theme switch based on your OS color scheme by adding the following snippet to your `settings.json`:
  ```json
  "window.autoDetectColorScheme": true,
  "workbench.preferredDarkColorTheme": "Darking Horse",
  "workbench.colorTheme": "Darking Horse",
  ```

### From within VS Code

- Go to `Preferences > Color Theme`.
- Search for _Darking horse_.

Alternatively:

- Go to the "Extensions" view, via `Preferences > Extensions`.
- Search for Darking Horse.

<br />
<br />

## Recommended setup

For the best, recommended experience use the following:

- [Iosevka font](https://typeof.net/Iosevka/)
- with the settings (you can paste these in your `settings.json`):
  ```json
  {
  	"breadcrumbs.enabled": true,
  	"editor.bracketPairColorization.enabled": true,
  	"editor.cursorStyle": "block",
  	"editor.fontFamily": "'Iosevka', monospace",
  	"editor.fontLigatures": true,
  	"editor.fontSize": 13,
  	"editor.guides.bracketPairs": true,
  	"editor.guides.bracketPairsHorizontal": "active",
  	"editor.minimap.enabled": false, // disable minimap
  	"editor.renderLineHighlight": "all",
  	"git.mergeEditor": false,
  	"terminal.integrated.fontFamily": "'Iosevka Term'",
  	"terminal.integrated.fontSize": 13,
  	"workbench.activityBar.visible": false, // hide activity bar
  	"workbench.colorCustomizations": {
  		"[Darking horse]": {
  			"editorLineNumber.foreground": "#333333"
  		}
  	},
  	"window.autoDetectColorScheme": true, // to enable auto theme switch based on OS color scheme
  	"workbench.preferredDarkColorTheme": "Darking Horse",
  	"workbench.colorTheme": "Darking Horse",
  	"workbench.panel.defaultLocation": "right", // place the default panel (terminal etc.) on the right
  	"workbench.settings.editor": "json",
  	"workbench.sideBar.location": "right", // place the sidebar on the right
  	"terminal.integrated.minimumContrastRatio": 1 // on certain themes, the color gets altered by VS Code for contrast, disable this to use Darking Horse colors
  }
  ```

## Overrides

To override this theme in your personal config file, please follow the guide in the [VS Code color theme documentation](https://code.visualstudio.com/api/extension-guides/color-theme). You could do something like this:

```json
// settings.json
{
	"workbench.colorCustomizations": {
		// So that this change is only for the Darking Horse theme
		"[Darking Horse]": {
			"editorLineNumber.foreground": "#333333"
		}
	}
},
```

## Issues

#### Terminal colors look weird!

This is because the [integrated terminal in VS Code has a minimum contrast ratio which dynamically changes the foreground color](https://code.visualstudio.com/updates/v1_66#_minimum-contrast-ratio-default-changed). This causes some foreground colors in _Darking Horse_ to be shown differently. You can add the following to your `settings.json` to override this:

```json
	"terminal.integrated.minimumContrastRatio": 1
```

## Development

Wanna try out customizing and contributing to _Karma_? Thanks! Here's how:

- Fork and clone this repository
- This project uses [pnpm](https://pnpm.io/)—make sure you've [installed and set it up](https://pnpm.io/installation) correctly!
- Install all the dependencies—these allow us to "hot reload" the theme during development.
  ```sh
  pnpm i
  ```
- Run the following command to start the `dev` script
  ```sh
  pnpm run dev
  ```
- Open this project in VS Code, and then go to `Run > Start Bebugging` or simply hit `F5`.

This opens up another instance of VS Code, with the "dev" version of Darking Horse! You can edit the color tokens in `src/tokens.ts` or change individual theme color variables in `src/generateTheme.ts`. Please make sure to use the [VS Code Theme Color reference](https://code.visualstudio.com/api/references/theme-color)!

## Credits

Darking Horse is inspired by a mix of [Ayu](https://marketplace.visualstudio.com/items?itemName=teabyii.ayu), Lucy and [Andromeda](https://marketplace.visualstudio.com/items?itemName=EliverLara.andromeda) themes. In addition, while starting work on the v3 release and on the lookout for a way to generate complimentary themes with tokens, I took heavy inspiration from [GitHub's VS Code themes](https://github.com/primer/github-vscode-theme).

The font used in all screenshots is [Iosevka](https://typeof.net/Iosevka/). 
If you like Darking Horse, thanks a lot! It truly means a lot to me. A 🌟star on the repository would be super cool! :)

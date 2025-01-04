<h1 align="center">
  <img width="120" height="120" src="https://github.com/user-attachments/assets/9af639b2-c553-43c8-ba07-d6c0f7f4fefa">
  <br>
  Pineapple Fried
</h1>


<p align="center">A customization pack for Zen Browser.</p>

<p align="center">Cohesion + Natsumi-Tweaks + Wazz-Tweaks</p>

![image](https://github.com/user-attachments/assets/52696e11-2e1c-4eb7-bae5-167ff04642ae)

## What is Pineapple Fried?
Pineapple Fried is a pack of customizations (a 'rice') made for [Zen Browser](https://zen-browser.app).

It integrates new UI styles, personal tweaks, and a compatibility layer for [Natsumi Browser](https://github.com/greeeen-dev/natsumi-browser/tree/main)

#

<br>

<div align="center">

Pineapple Fried has been tested on these versions of Zen:

| Build | Version | Date |
| ------ | ------ | ------|
| **Beta** | `1.0.2-b.5` | Dec. 26, 2024 |
| **Twilight** | `1.6t` | Jan. 03, 2025 |

</div>

<br>

## Features
### Cohesion
Cohesion adds an integrated URL style, transparent newtab pages, and a *cohesive* transparent look to the various bars and panels

[![](https://github.com/user-attachments/assets/e19e1a3d-c3ea-42a1-a655-4b9353463ca5)](https://github.com/user-attachments/assets/e19e1a3d-c3ea-42a1-a655-4b9353463ca5)

<br>

### Natsumi Tweaks
Get the stylish appearance, animations, and features of [Natsumi Browser](https://github.com/greeeen-dev/natsumi-browser/tree/main), made compatible with Cohesion with some personal tweaks. 

**This is a compatibility layer that only works if regular Natsumi is already installed.*

![image](https://github.com/user-attachments/assets/dad73ffd-36c0-4fe5-ad86-db207d900bf5)

<br>

### Wazz-Tweaks
More personal changes with some community additions.

![image](https://github.com/user-attachments/assets/65e6e6f7-da21-489a-a8c6-aa97572420e2)

<br>


# Installation
**Pineapple Fried** and its components are not available on the Zen Mods page, as this isn't intended to be a Mod. You will need to
install it by copying the files to your profile's chrome folder. Here's a step-by-step guide to follow:

1. userChrome.css
2. userContent.css
3. Brower Configs (in about:config)
4. Zen Settings
5. Toolbar layout
6. Mods
7. Browser Transparency
8. Gradients (optional)
9. Extensions (optional)

#

<br>

## userChrome.css

1. If you have not already, follow the [Zen Live Editing](https://docs.zen-browser.app/guides/live-editing) guide to first make your own **chrome** folder.

2. Download the **"cohesion"**, **"natsumi-tweaks"**, and **"wass-tweaks"** folders from above and drop them into your **"chrome"** folder. 

3. Add these import statements to your **userChrome.css** (*or download the userChrome.css file from above and place it in your **chrome** folder*):
```
/* Wazz-Tweaks */
@import "wazz/wazz.css";

/* Cohesion */
@import "cohesion/cohesion.css";

/* Natsumi-Tweaks */
@import "natsumi-tweaks/natsumi-tweaks.css";
```
> [!Note]
> - Remove any of my personal CSS / Cohesion CSS from your **userChrome.css** file if you have previously used it.
> - It's now all being called via the import statements in your **userChrome.css** file.
> - You may still add other custom CSS to your userChrome.css underneath the imports.
> - You can Live Edit mod files, just search for the Module name in the Style Browser (Ctrl+Alt+Shift+I)

## userContent.css



## Browser configs (in about:config)
These are the configs you need to use. If they do not exist, type the config and click the **+** button to create it.

### Zen Options
- `browser.tabs.allow_transparent_browser` = `true`*
- `zen.workspaces.show-workspace-indicator` = `false`
  
>[!Note]
>**Websites without a background will display the browser UI underneath the content.*
>
>*Extensions like [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) fix this by setting their own background.*

### Natsumi options
- `natsumi.theme.clip-path-force-polygon`: `true`
- `natsumi.sidebar.blur-zen-sidebar`: `true`
- `natsumi.sidebar.containers-no-inactive-border`: `true`
- `natsumi.sidebar.enable-tab-groups`: `true`*
- `natsumi.sidebar.zen-sidebar-glass-effect`: `true`



## FAQs
### "Can I use other userchromes with Pineapple Fried?"
Sure! Just paste it right below the Pineapple Fried loader (userChrome.css) and you can use your own
userchrome alongside Pineapple Fried.

### "Can I disable individual features?"
You're free to disable loading certain modules (CSS files) if you feel like it. But Natsumi will still need
to load config.css, natsumi/preload.css and natsumi/postload.css for things to work.

### "Why is userChrome.css so empty?"
Pineapple Fried uses a system where the userChrome.css file acts as a loader that loads the skin,
instead of being the file that contains all rules. This way, it's easier for users to quickly enable and
disable custom CSS. This system is reffered to as **uCL** (**u**ser**C**hrome **L**oader).

## Troubleshooting
### "I don't see any of the Natsumi options in about:config!"
These are custom options which you need to create. Type in the exact name, then press the plus button on
the right to create the config.

### "Tab groups aren't working!"
> [!WARNING]
> The developer of Zen Browser recommends **against** using custom CSS to implement Tab Groups like
> Natsumi's for the time being. Proceed at your own risk.

Set `browser.tabs.groups.enabled` and `natsumi.sidebar.enable-tab-groups` to true.

### "Something's bugged!"
There may be Zen Mods or userchromes that you're using alongside Pineapple Fried that breaks things.
Please disable these then try again.

If the issue still persists, open an issue or report the bug to the developer through Discord.

## Acknowledgements
Thank you to:
- [greeeen-dev](https://github.com/greeeen-dev) for the incredible work in [Natsumi Browser](https://github.com/greeeen-dev/natsumi-browser/tree/main)
- [asev](https://github.com/lunar-os) for ZenCss, which served as the base for Natsumi Browser's base
  CSS for v1
- [vicky5124](https://github.com/vicky5124) for the Tab Groups CSS
- [mr-cheff](https://github.com/mr-cheff) and Zen's
  [contributors](https://github.com/zen-browser/desktop/graphs/contributors) for creating Zen Browser

<h1 align="center">
  <img width="120" height="120" src="https://github.com/user-attachments/assets/9af639b2-c553-43c8-ba07-d6c0f7f4fefa">
  <br>
  Pineapple Fried
</h1>


<p align="center">
  A customization pack for Zen Browser
  <br>
  Cohesion + Natsumi-Tweaks + Wazz-Tweaks
  <br>
  <a href="https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#what-is-pineapple-fried">What is Pinneapple Fried?</a> | <a href="https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#features-included">Features Included</a> | <a href="https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#installation">Installation</a> | <a href="https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#faq">FAQ</a> | <a href="https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#acknowledgements">Acknowledgements</a>
</p>

https://github.com/user-attachments/assets/862fdebd-4dd5-4953-97b7-22decc4fd59c

## What is Pineapple Fried?
Pineapple Fried is a pack of customizations (a 'rice') made for [Zen Browser](https://zen-browser.app).

It integrates new UI styles, personal tweaks, and a compatibility layer for [Natsumi Browser](https://github.com/greeeen-dev/natsumi-browser/tree/main)

<br>

<div align="center">

Pineapple Fried has been tested on these versions of Zen:

| Build | Version | Date |
| ------ | ------ | ------|
| **Beta** | `1.0.2-b.5` | Dec. 26, 2024 |
| **Twilight** | `1.6t` | Jan. 03, 2025 |

</div>

## Features Included

<h3 align="left">
  <img width="80" height="80" src="https://github.com/user-attachments/assets/242e9477-3149-473a-8c1d-655476f7dba3">
  <br>
  Cohesion
</h3>

Cohesion adds an integrated URL style, transparent newtab pages, and a *cohesive* transparent look to the various bars and panels

https://github.com/user-attachments/assets/2bf31d3a-18e0-4405-9389-8d0f036127a4

<br>

<h3 align="left">
  <img width="80" height="80" src="https://github.com/user-attachments/assets/a44b390d-4c25-474a-af08-434d81cd34dc">
  <br>
  Natsumi-Tweaks
</h3>

Get the stylish appearance, animations, and features of [Natsumi Browser](https://github.com/greeeen-dev/natsumi-browser/tree/main), made compatible with Cohesion with some personal tweaks. 

**This is a compatibility layer. It requires Natsumi to already be installed.*

![image](https://github.com/user-attachments/assets/dad73ffd-36c0-4fe5-ad86-db207d900bf5)

<br>

<h3 align="left">
  <img width="80" height="80" src="https://github.com/user-attachments/assets/ebeb7514-9984-40db-a81f-6b1bb5cc50ff">
  <br>
  Wazz-Tweaks
</h3>

More personal changes with some community additions.

![image](https://github.com/user-attachments/assets/65e6e6f7-da21-489a-a8c6-aa97572420e2)

<br>


# Installation
**Pineapple Fried** and its components are not available on the Zen Mods page, as this isn't intended to be a Mod. You will need to
install it by copying the files to your profile's chrome folder. Here's a step-by-step guide to follow:

1. [userChrome.css](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#1-userchromecss)
2. [userContent.css](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#2-usercontentcss)
3. [Brower Configs (in about:config)](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#3-browser-configs-in-aboutconfig)
4. [Zen Settings](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#4-zen-settings)
5. [Toolbar layout](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#5-toolbar-layout)
6. [Mods](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#6-mods)
7. [Browser Transparency](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#7-browser-transparency)
8. [Gradients](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#8-gradients) (optional)
9. [Extensions](https://github.com/TheBigWazz/Pineapple-Fried/blob/main/README.md#9-extensions) (optional)

#

*The following guide assumes Natsumi Browser is already installed.*

<br>

## 1. userChrome.css

**a):** If you have not already, follow the [Zen Live Editing](https://docs.zen-browser.app/guides/live-editing) guide to first make your own **chrome** folder.

**b):** Download the **"cohesion"**, **"natsumi-tweaks"**, and **"wass-tweaks"** folders from above and drop them into your **"chrome"** folder. 

**c):** Add these import statements to **userChrome.css** (*or download the userChrome.css file from above and place it in your **"chrome"** folder*):
```
@import "Cohesion/Cohesion.css";

@import "natsumi/natsumi.css";

@import "Wazz/Wazz.css";

@import "natsumi-tweaks/natsumi-tweaks.css";
```
> [!Note]
> - Remove any of my personal CSS / Cohesion CSS from your **userChrome.css** file ***if you have previously used it.***
> - It's now all being called via the import statements in your **userChrome.css** file.
> - You may still add other custom CSS to your userChrome.css underneath the imports.
> - You can Live Edit mod files, just search for the Module name in the Style Browser (Ctrl+Alt+Shift+I)

<br>

## 2. userContent.css

**a):** Download the **"zen-new-tab"** folder from above and drop it into your **"chrome"** folder

**b):** Add these import statements to **"userContent.css"** (*or download the userContent.css file from above and place it in your **"chrome"** folder*):
```
/* zen new tabs */
@import "zen-new-tabs/zen-new-tabs.css";

/* Natsumi Pages */
@import "natsumi-pages/natsumi-pages.css";
```

<br>

## 3. Browser configs (in about:config)

These are the configs you need to use. If they do not exist, type the config and click the **+** button to create it.

### **a):** Zen Options
- `browser.tabs.allow_transparent_browser` = `true`*
- `zen.workspaces.show-workspace-indicator` = `false`
  
>[!Note]
>**Websites without a background will display the browser UI underneath the content.*
>
>*Extensions like [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) fix this by setting their own background.*

### **b):** Natsumi options
- `natsumi.theme.clip-path-force-polygon`: `true`
- `natsumi.sidebar.blur-zen-sidebar`: `true`
- `natsumi.sidebar.containers-no-inactive-border`: `true`
- `natsumi.sidebar.enable-tab-groups`: `true`*
- `natsumi.sidebar.zen-sidebar-glass-effect`: `true`

<br>

## 4. Zen Settings

**a):** Look and Feel 
  - Select '__Multiple Toolbars__'
  - Uncheck '__Show New Tab Button on Tab List__'
  - Uncheck '__Show border for the bottom icons__'
  - Zen URL bar Behavior = Normal
    
**b):** Tab Management
  - Check '__Hide the default container indicator in the tab bar__'
  - Check '__Allow workspaces have their own pinned tabs__'
  - Check '__Display workspaces as an icon strip__'
    
**c):** Home 
  - Homepage and new windows: Firefox Home (default)
  - New tabs: Firefox Home (default)

<br>

## 5. Toolbar Layout

- Right click on the Tab Bar and select 'Customize Toolbar'
- Click and drag items to arrange them in this same order:

![image](https://github.com/user-attachments/assets/bf7919db-9e69-4aa5-8bfb-2a21d8da7813)

`Account` | `Bookmark toolbar items` | `4x Spacers` | `Nav buttons` | `URL Bar` | `Copy URL button` | `4x Spacers`

<br>

## 6. Mods

* [Bottom Essentials](https://zen-browser.app/mods/477bc813-c333-4747-813e-00e0420ceec0)
* [Better Unloaded Tabs](https://zen-browser.app/mods/f7c71d9a-bce2-420f-ae44-a64bd92975ab)
* [Cleaner Extension Menu](https://zen-browser.app/mods/1e86cf37-a127-4f24-b919-d265b5ce29a0)
* [Cleaned URL Bar](https://zen-browser.app/mods/a5f6a231-e3c8-4ce8-8a8e-3e93efd6adec)
* [Floating Status Bar](https://zen-browser.app/mods/906c6915-5677-48ff-9bfc-096a02a72379)
* [Hide Extension Name](https://zen-browser.app/mods/cb15abdb-0514-4e09-8ce5-722cf1f4a20f)
* [Midnight](https://zen-browser.app/mods/5ca67725-1f43-4ff2-9fcf-0c59af71c73a)
* [Only Close On Hover](https://zen-browser.app/mods/4596d8f9-f0b7-4aeb-aa92-851222dc1888)
* [SuperPins](https://zen-browser.app/mods/ad97bb70-0066-4e42-9b5f-173a5e42c6fc)

  **SuperPins Settings:**
  * [x] Makes pinned tabs look similar to Essentials (icon only in a grid)
  * [x] Adds a background to the pinned tabs
  * Select the gap between Essentials: ```Normal```
* [Super URL Bar](https://zen-browser.app/mods/d93e67f8-e5e1-401e-9b82-f9d5bab231e6)

  **Super URL Bar Settings:**
  * Centeres the text inside the URL Bar: ```Always Centered```
  * Enable a background blur when the URL bar is focused & select its intensity: ```Really Strong```
  * [x] Always open websites in a new tab when using url bar

<br>

## 7. Browser Transparency

### Windows 11

#### **- Mica For Everyone**

- Download and install from their repo: https://github.com/MicaForEveryone/MicaForEveryone
- After installing, open and click the '__+__' button in the bottom left corner
- Click '__Add Process Rule__'
- Type `zen`
- Select `zen` in the list on the left
- Style Settings:
  - Titlebar Color: `Default`
  - Backdrop Type: `Mica`
  - Corner Mode: `Default`
- Advanced:
  - Extend Frame Into Client Area: `Off`
  - Blur Behind: `On`

### Alternitives

| OS | Link |
| --- | --- |
| Windows 10 | [DWMBlurGlass](https://github.com/Maplespe/DWMBlurGlass) |
| MacOS | Something |
| Linux | |
| - KDE | [KWin Better Blur](https://github.com/taj-ny/kwin-effects-forceblur) |
| - Gnome | [Blur My Shell](https://github.com/aunetx/blur-my-shell) |

<br>

## 8. Gradients (optional)

If you like the colors you see in the screenshots above, you can manually copy these gradient settings. 

To edit gradient, right click Tab Bar and select `Change Theme Color`.

![image](https://github.com/user-attachments/assets/fb165906-7601-4421-8a52-40b8dc3441e9)

![image](https://github.com/user-attachments/assets/db37488d-a723-41d2-9ff2-ff7e21459608)

![image](https://github.com/user-attachments/assets/bbe4fff5-982a-4324-bb77-3e73e4b2fa05)

<br>

## 9. Extensions (optional)
* [Copy Tab URL](https://addons.mozilla.org/en-US/firefox/addon/zen-copy-tab-url/) *Adds the Copy URL button to the URL bar.*
* [Proton Pass](https://addons.mozilla.org/en-US/firefox/addon/proton-pass/) *Is the purple diamond at the far left of the URL bar.*
* [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) *Fixes missing backgrounds on websites.*

<br>

# FAQ
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

# Troubleshooting
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

# Acknowledgements
Thank you to:
- [greeeen-dev](https://github.com/greeeen-dev) for the incredible work in [Natsumi Browser](https://github.com/greeeen-dev/natsumi-browser/tree/main)
- [asev](https://github.com/lunar-os) for ZenCss, which served as the base for Natsumi Browser's base
  CSS for v1
- [vicky5124](https://github.com/vicky5124) for the Tab Groups CSS
- [mr-cheff](https://github.com/mr-cheff) and Zen's
  [contributors](https://github.com/zen-browser/desktop/graphs/contributors) for creating Zen Browser

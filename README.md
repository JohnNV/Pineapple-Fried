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

![image](https://github.com/user-attachments/assets/dad73ffd-36c0-4fe5-ad86-db207d900bf5)

<br>

### Wazz-Tweaks
More personal changes with some community additions.

![image](https://github.com/user-attachments/assets/65e6e6f7-da21-489a-a8c6-aa97572420e2)

<br>


## Installation
**Pineapple Fried** and its components are not available on the Zen Mods page, as this isn't intended to be a Mod. You will need to
install it by copying the files to your profile's chrome folder.

### Natsumi-Tweaks
#### If you already have a userChrome.css file
1. Copy natsumi-config.css and natsumi folder to your chrome folder.
2. Add `@import "natsumi/natsumi.css";` to the beginning of your userChrome.css file.
3. Restart Zen Browser and enjoy!

#### If you don't have a userChrome.css file
1. Create a new chrome folder in your profile folder, if you haven't already.
   ([guide](https://docs.zen-browser.app/guides/live-editing))
2. Copy userChrome.css to the chrome folder.
3. Copy natsumi-config.css and natsumi folder to the chrome folder.
4. Restart Zen Browser and enjoy!

### Natsumi Browser Pages
#### If you already have a userContent.css file
1. Add `@import "natsumi-pages/natsumi-pages.css";` to the beginning of your userContent.css file.
2. Restart Zen Browser and enjoy!

#### If you don't have a userContent.css file
1. Create a new chrome folder in your profile folder, if you haven't already.
   ([guide](https://docs.zen-browser.app/guides/live-editing))
2. Copy userContent.css to the chrome folder.
3. Copy natsumi-config.css to the chrome folder, if you haven't already.
4. Copy natsumi-pages folder to the chrome folder.
5. Restart Zen Browser and enjoy!

## Browser configs (in about:config)
These are the configs you can use to tweak Natsumi Browser. If you want to tweak the animation duration
and delay, change the variables in the config.css file.

### Base theme
- `natsumi.theme.clip-path-force-polygon`: Uses polygon instead of inset for URLbar and Zen Sidebar
  blurring. Enable this if you need this for compatibility with other userchromes/Mods like
  [Cohesion](https://github.com/TheBigWazz/ZenThemes/tree/main/Cohesion).
- `natsumi.theme.disable-blur`: Disables blurring for glass effects. Use this if Zen Browser lags
  too much.
- `natsumi.theme.disable-glass-shadow`: Disables shadow for glass effects.
- `natsumi.theme.disable-loading-animations`: Disables loading animation for tabs.
- `natsumi.theme.disable-urlbar-animation`: Disables URLbar loading animation for tabs.
- `natsumi.theme.enable-border-animation`: Enables border loading animation for tabs. This may use up
  quite some GPU.
- `natsumi.theme.fullscreen-glass-effect`: Enables glass effect for full screen popup message.

### URLbar
- `natsumi.urlbar.disabled`: Disables Natsumi URLbar and reverts the URLbar style back.
- `natsumi.urlbar.disable-transparency`: Disables URLbar background transparency.
- `natsumi.urlbar.force-nowrap`: Prevents wrapping to make things more compact regardless of window
  width.
- `natsumi.urlbar.light`: Disables some animations to make Natsumi URLbar lighter.

### Navbar
- `natsumi.navbar.floating-navbar`: Makes the navbar float on compact mode.
- `natsumi.navbar.glass-effect`: Adds glass effect for the navbar on compact mode.

### Sidebar
- `natsumi.sidebar.blur-zen-sidebar`: Blurs Zen Sidebar background. This may cause some lag when you
  have both Zen Sidebar and Natsumi URLbar opened at the same time.
- `natsumi.sidebar.containers-dashed-border`: Uses dashed border for container tabs instead of solid
  border. Selected tabs will always use solid border.
- `natsumi.sidebar.containers-thicker-gradient`: Makes container tabs indicator gradient "thicker".
- `natsumi.sidebar.containers-no-inactive-border`: Hides the container tabs indicator border when the
  tab is not selected.
- `natsumi.sidebar.disable-bigger-tab-label`: Disables bigger tab labels and reverts them back to the
  normal font size.
- `natsumi.sidebar.disable-panel-transparency`: Disables transparent background for sidebar panels
  (e.g. Bookmarks).
- `natsumi.sidebar.enable-tab-groups`: Enables Tab Groups CSS. This is opt-in as the developer does
  not recommend using custom CSS to implement Tab Groups at the moment.
- `natsumi.sidebar.floating-panel`: Makes the Firefox sidebar panel float.
- `natsumi.sidebar.panel-glass-effect`: Adds glass effect to Firefox sidebar panel.
- `natsumi.sidebar.panel-position-center`: Vertically centers Firefox sidebar panel if it is floating.
- `natsumi.sidebar.panel-position-bottom`: Moves Firefox sidebar panel to the bottom if it is floating.
  Overrides `natsumi.sidebar.panel-position-center` if enabled.
- `natsumi.sidebar.panel-resizable`: Makes the Firefox sidebar panel resizable.
- `natsumi.sidebar.tabs-glass-effect`: Adds glass effect for the sidebar on compact mode.
- `natsumi.sidebar.unlimited-pinned-tabs`: Removes the limit on the maximum number of tabs being shown
  in the pinned section of the vertical tabs.
- `natsumi.sidebar.zen-sidebar-glass-effect`: Adds glass effect to Zen Sidebar.
- `natsumi.sidebar.container-tabs-border`: Adds a border to all tabs irrespective of whether it's the
  active tab or not.

### Findbar
- `natsumi.findbar.disabled`: Disables Natsumi Findbar and reverts the findbar style back.
- `natsumi.findbar.disable-not-found-bg`: Disables red background that appears when there are no
  results.
- `natsumi.findbar.wider-findbar`: Increases maximum Findbar width back to 720px.

### PDF Viewer
- `natsumi.pdfjs.disabled`: Disables Natsumi PDF Viewer and reverts the PDF viewer back.

### Home
- `natsumi.home.disabled`: Disables Natsumi FF home and reverts the FF home page back.
- `natsumi.home.custom-background`: Uses the custom background set in config as the home screen
  background.

### Global tweaks
- `natsumi.global.highlight-accent-color`: Uses the accent color for highlighting.

### Experiments
- `natsumi.experiments.compact-bounce`: Adds a bounce effect to the tabs sidebar in compact mode.
- `natsumi.experiments.resizable-tabs`: Makes tabs horizontally resizable. Doesn't work that well though.

## FAQs
### "Mod xyz has a similar look as Natsumi, did they copy you?"
Like I've said in the Features section, Natsumi's base UI CSS comes from asev's ZenCss repository.
This is actually a very popular userchrome among the Zen Browser community, so it's likely that the
Mod also uses the same userchrome I used.

### "Can I use other userchromes with Natsumi?"
Sure! Just paste it right below the Natsumi Browser loader (userChrome.css) and you can use your own
userchrome alongside Natsumi Browser.

### "Can I disable individual features?"
You're free to disable loading certain modules (CSS files) if you feel like it. But you will still need
to load config.css, natsumi/preload.css and natsumi/postload.css for things to work.

### "Why is userChrome.css so empty?"
Natsumi Browser uses a system where the userChrome.css file acts as a loader that loads the skin,
instead of being the file that contains all rules. This way, it's easier for users to quickly enable and
disable custom CSS.

## Troubleshooting
### "URLbar blur won't work!"
Make sure both `layout.css.backdrop-filter.enabled` and `layout.css.backdrop-filter.force-enabled` are
set to true. Also make sure that you're using WebRender and hardware rendering.

### "Zen Browser lags a lot!"
This may be due to the URLbar blurring or animations (likely the blur). Set `natsumi.theme.disable-blur`
to false to disable the blur, and `natsumi.urlbar.light` to true to disable the animations.

### "I don't see any of the Natsumi options in about:config!"
These are custom options which you need to create. Type in the exact name, then press the plus button on
the right to create the config.

### "Tab groups aren't working!"
> [!WARNING]
> The developer of Zen Browser recommends **against** using custom CSS to implement Tab Groups like
> Natsumi's for the time being. Proceed at your own risk.

Set `browser.tabs.groups.enabled` and `natsumi.sidebar.enable-tab-groups` to true.

### "Something's bugged!"
There may be Zen Mods or userchromes that you're using alongside Natsumi Browser that breaks things.
Please disable these then try again.

If the issue still persists, open an issue or report the bug to the developer through Discord.

## Acknowledgements
Thank you to:
- [asev](https://github.com/lunar-os) for ZenCss, which served as the base for Natsumi Browser's base
  CSS for v1
- [vicky5124](https://github.com/vicky5124) for the Tab Groups CSS
- [mr-cheff](https://github.com/mr-cheff) and Zen's
  [contributors](https://github.com/zen-browser/desktop/graphs/contributors) for creating Zen Browser

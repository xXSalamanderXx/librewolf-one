# LibreWolf-ONE

An Opera One-inspired theme for LibreWolf, based on [Firefox-ONE](https://github.com/Godiesc/firefox-one) by [Godiesc](https://github.com/Godiesc).

![LibreWolf-ONE preview](https://i.postimg.cc/R0pFTnDp/Screenshot-2026-06-18-050954.png)

## Credits 🙏

The original theme and most of the underlying customization work are maintained by [Godiesc](https://github.com/Godiesc) for [Firefox-ONE](https://github.com/Godiesc/firefox-one) and it's contributors.

This repository is a LibreWolf-focused fork which closely follows upstream. All Firefox branding throughout the theme has been changed to Librewolf branding.

## Installation 🧑‍🎨

1. Download the theme from the [Releases](https://github.com/xXSalamanderXx/librewolf-one/releases) page.
2. Extract the downloaded archive.
3. Open LibreWolf and enter `about:support` in the address bar.
4. Find the Profile Directory or Profile Folder entry and open that location. You can also use `about:profiles` to locate the correct profile.
5. Back up your existing `chrome` folder and `user.js` file, if present.
6. Close LibreWolf completely.
7. Copy the theme's `chrome` folder and `user.js` file into your profile directory.
   - If you already use a custom `user.js`, merge the theme's preferences rather than overwriting your existing configuration.
   - Make sure the `chrome` folder is directly inside the profile directory, not inside an additional extracted folder.
8. Start LibreWolf and install one of the compatible themes listed below.
9. Restart LibreWolf to apply the configuration.

> The repository's latest development code may target newer browser versions. Prefer a release when available, and check its compatibility notes before installing.

## Compatible Themes

### Adaptive Theme

- [🧿 Light/Dark Adaptive](https://addons.mozilla.org/en-US/firefox/addon/beautiful-focused-tab/)

### Colour Variants

| Theme | Theme |
|---|---|
| [🔴 Fuchsia](https://addons.mozilla.org/en-US/firefox/addon/beautiful-opera-gx-fucsia/) | [🔵 Blue](https://addons.mozilla.org/en-US/firefox/addon/beautiful-opera-gx-blue/) |
| [🟢 Green](https://addons.mozilla.org/en-US/firefox/addon/beautiful-gx-green/) | [🖍 Poison](https://addons.mozilla.org/en-US/firefox/addon/beautiful-poison/) |
| [🎑 Swamp](https://addons.mozilla.org/en-US/firefox/addon/beautiful-swamp-in-autumn/) | [🌈 Red Blur](https://addons.mozilla.org/en-US/firefox/addon/beautiful-red-blur/) |
| [🌆 Purple Sky](https://addons.mozilla.org/en-US/firefox/addon/beautiful-purple-sky/) | [💜 Purple](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-witchcraft-purple/) |
| [💚 Aquamarine](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-electric-aquamarine/) | [🦧 Orange](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-ember-orange/) |
| [💠 Cyan](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-frozen-cyan/) | [🍏 Light Green](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-level-up-green/) |
| [💛 Yellow](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-stamina-yellow/) | [🗻 Grey](https://addons.mozilla.org/en-US/firefox/addon/opera-gx-wizard-grey/) |

### Light Themes

- [⚪🔴 Fuchsia](https://addons.mozilla.org/en-US/firefox/addon/opera-light/)
- [⚪🔵 Waves](https://addons.mozilla.org/en-US/firefox/addon/beautiful-waves/)

See the upstream [video explanation](https://imgur.com/a/0ZASdRb) for switching between light and dark appearances when needed.

## Important Information ⚠️

- Use flexible spaces in the Customize Toolbar screen to add separation between toolbar items.
- The theme uses the bookmarks toolbar for its left sidebar. Keep the bookmarks toolbar enabled when using the sidebar layout.
- Browser updates can affect custom interface themes. Updates usually address this before visual defects occur.

### Sidebar Extensions

The upstream project lists the following extensions for use with its sidebar layout:

- [Twitch](https://addons.mozilla.org/en-US/firefox/addon/twitch-live-channels/)
- [WhatsApp](https://addons.mozilla.org/en-US/firefox/addon/chatwapp-in-sidebar/)
- [Telegram](https://addons.mozilla.org/en-US/firefox/addon/telegram-in-sidebar/)
- [Facebook Messenger](https://addons.mozilla.org/en-US/firefox/addon/messenger-sidebar-with-toolbar/)
- [Twitter](https://addons.mozilla.org/en-US/firefox/addon/twitter-as-a-sidebar/)
- [Instagram Chat](https://addons.mozilla.org/en-US/firefox/addon/instachat-in-sidebar/)
- [Discord](https://addons.mozilla.org/en-US/firefox/addon/discord-in-sidebar/)
- [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)
- [Simple Tab Groups](https://addons.mozilla.org/en-US/firefox/addon/simple-tab-groups/)

These are optional third-party extensions. Their availability and compatibility are maintained by their respective developers.

## Optional Features 🔨

Open `about:config` and create or update the following Boolean preferences as needed.

| Feature | Preference | Value |
|---|---|---|
| Disable the left sidebar | `firefoxone.style_without_leftsidebar` | `true` |
| Disable the default colours | `firefoxone.without-default-colors` | `true` |
| Enable tree-style tabs | `firefoxone.tree_tabs_style` | `true` |
| Expand vertical tabs on hover | `firefoxone.verticalTabs-expandOnHover` | `true` |
| Add a gradient border to the selected tab | `firefoxone.selected_tab_gradient_border` | `true` |
| Enable images in menus | `firefoxone.image_in_menus` | `true` |
| Enable the main image | `firefoxone.main-image` | `true` |
| Enable the rhythm image for tabs playing audio | `firefoxone.rhythm_sound_tab` | `true` |

To use tree-style tabs without the left sidebar, enable both:

| Preference | Value |
|---|---|
| `firefoxone.tree_tabs_style` | `true` |
| `firefoxone.style_without_leftsidebar` | `true` |

For screenshots and configuration examples, see the upstream [feature previews](https://github.com/Godiesc/firefox-one/tree/main/Previews).

## Customization 

### Layout and Appearance

Edit [`chrome/components/one_root-personal.css`](chrome/components/one_root-personal.css) to customize options such as:

- Wallpapers.
- Tab and toolbar height.
- Left-sidebar width.
- New-tab wordmark colour.
- Visibility of the browser logo and new-tab search bar.

Read the comments beside each variable before changing it.

### New-Tab Wallpapers

The theme stores its bundled wallpapers in [`chrome/newtab`](chrome/newtab).

You can replace the bundled images while preserving their filenames, or update the wallpaper references in `one_root-personal.css`.

The upstream project also provides a [wallpaper gallery](https://imgur.com/a/j78IhJN).

### Wallpapers for Internal Pages

The default internal-page wallpapers are:

- `wallpaper-dark1.png`
- `wallpaper-light1.png`

Replace these files in `chrome/newtab`, or change their references in `one_root-personal.css`.

### Accent Colour

Change the `--general-color` variable in `one_root-personal.css` to customize the accent colour used by the theme's internal-page styling.

Restart LibreWolf after making changes.

## Compatibility

The following platform results were documented by the upstream Firefox-ONE project. They are historical upstream reports, not a guarantee of compatibility with current LibreWolf releases.

| Platform | Upstream Status |
|---|---|
| Linux — Gnome & KDE Plasma | Reported tested ✅️ |
| Windows 11 | Reported tested ✅️ |
| Windows 10 | Reported tested ✅️ |
| macOS | Reported tested ✅️ |

### Platform Previews (from Firefox-One)

- [Linux — Manjaro KDE](https://imgur.com/a/Di7Db9z)
- [Windows 10](https://github.com/Godiesc/firefox-one/assets/22057609/55e39c67-7588-456a-a30b-278f1dc4bd19)
- [Windows 11](https://imgur.com/a/WhypdHU)
- [macOS](https://imgur.com/a/UQ1TiUr)

## Issues

If you encounter a problem, include your LibreWolf version, operating system, enabled theme options, and a screenshot when opening an [issue](https://github.com/xXSalamanderXx/librewolf-one/issues).

## Related Project

For another Opera-inspired browser theme by the original developer, see [Firefox-GX](https://github.com/Godiesc/firefox-gx).

## Finding Your Profile Directory

Open `about:support` and locate the Profile Directory or Profile Folder entry.

Alternatively, open `about:profiles` to view your profiles and their root directories.

See the upstream [profile-directory example](https://github.com/Godiesc/firefox-one#example-of-aboutsupport) for a visual reference.

---

<p align="center">
  <b>⭐ Star the repo • ☕ Support development • 🚀 Explore more projects</b>
</p>

## ⭐ Show Your Support

If this repo has helped you, please consider giving it a star on GitHub! It helps show support, motivates future updates, and encourages continued development. 🚀

Every ⭐ makes a difference. Thanks for helping this project grow! 🙌

Please also consider starring [Godiesc's original Firefox-ONE project](https://github.com/Godiesc/firefox-one).

## ☕ Support Development

If you'd like to support my work on this fork and my other projects, you can buy me a coffee here:

[☕ buymeacoffee.com/SinZZzz](https://buymeacoffee.com/SinZZzz)

Your support is appreciated. 💙

This support link belongs to the maintainer of this fork, not the original Firefox-ONE developer.

## 🔍 Check Out My Repos

You might also like these projects:

- [🦁 SlimBrave](https://github.com/xXSalamanderXx/SlimBrave)
- [🦎 salamander-trackers](https://github.com/xXSalamanderXx/salamander-trackers)
- [📜 Salamander-Userscripts](https://github.com/xXSalamanderXx/Salamander-Userscripts)
- [🔎 RLSBB-Search-Plus](https://github.com/xXSalamanderXx/RLSBB-Search-Plus)
- [🎬 HDEncode-Search-Plus](https://github.com/xXSalamanderXx/HDEncode-Search-Plus)
- [📷️ Caesium Image Compressor - Linux](https://github.com/xXSalamanderXx/caesium-image-compressor-linux)
- [📚 Arvio-Catalogs](https://github.com/xXSalamanderXx/Arvio-Catalogs)

---

## Disclaimer

This project is provided as-is, without warranties, as described in the license.

Back up your browser profile before installing or modifying custom interface files. You are responsible for the changes you make to your configuration.

This is an independent community theme and is not affiliated with or endorsed by LibreWolf, Mozilla, or Opera.

The applicable warranty disclaimers and limitations of liability are set out in the [license](LICENSE).

## License 📄

This project is licensed under the Mozilla Public License 2.0 (MPL-2.0).

The original Firefox-ONE theme was created by [Godiesc](https://github.com/Godiesc). Original copyright and license notices remain applicable.

See the full license here: [Mozilla Public License 2.0](https://github.com/xXSalamanderXx/librewolf-one/blob/main/LICENSE).

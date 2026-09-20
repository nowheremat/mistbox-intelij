# Mistbox
<!-- Plugin description -->
## Description

**Mistbox** is a pair of muted, easy-on-the-eyes themes (**Dark Mistbox** and **Light Mistbox**) for IntelliJ-based IDEs, built for the modern **Islands (New UI)** aesthetic.

Its palette was sampled from a Zed + Ghostty setup: a cool near-black background, neutral grey text and comments, periwinkle keywords, mint types, soft green strings and pale steel-blue functions.

### Current Status

| Theme Variant | Status |
| :--- | :--- |
| **Dark Mistbox** | ✅ **Available** |
| **Light Mistbox** | ✅ **Available** |

### Features

#### Designed for the "Islands" UI
Toolbars, project trees and editor tabs are tuned for the **New UI** (Islands), so the whole window blends with the palette.

#### Editor scheme included
A dedicated editor color scheme covers Java, Kotlin, Go, Python, JavaScript, Rust, HTML/CSS, YAML and more. Comments stay italic; method calls stay upright.

---
<!-- Plugin description end -->

### Installation

1. Open **Settings/Preferences** in your IDE.
2. Navigate to **Plugins**, click the gear icon and choose **Install Plugin from Disk...**
3. Pick the zip from `build/distributions/` (see *Development* below).
4. Go to **Appearance & Behavior** > **Appearance** and select **Dark Mistbox** or **Light Mistbox** from the Theme dropdown.

### Development

```
./gradlew runIde        # launches a sandbox IDE with the theme
./gradlew buildPlugin   # creates build/distributions/*.zip
./gradlew verifyPlugin  # runs the plugin verifier
```

Colors live in two places: the `colors` block of `themes/mistbox-<variant>/mistbox-<variant>.json` (UI) and
`mistbox-<variant>.xml` (editor). `palette-dark.csv` lists every named UI color.

### Palette notes

The main colors were measured from a compressed screenshot, so treat them as close approximations:

| Role | Color |
| :--- | :--- |
| Background | `#13171A` |
| Text | `#CDCFD1` |
| Comments | `#84898B` |
| Keywords / accent | `#9AA0C5` |
| Strings | `#9BC392` |
| Types | `#9DCFC3` |
| Constants | `#9ECCB6` |
| Functions | `#9DB6C0` |
| Numbers | `#DE9A85` (estimated) |

### Acknowledgments

The project layout and theme-key coverage follow [gruvbox-material-island-theme](https://github.com/nowheremat/gruvbox-material-island-theme) (MIT)

***This plugin is not affiliated with or endorsed by JetBrains.***


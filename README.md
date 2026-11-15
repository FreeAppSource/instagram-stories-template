# Instagram Stories Template

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Hugo** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `instagram-template-ios-hugo.sketch` by **Hugo**: one route per artboard, with the artboard's layout, colours, images and text.

![Instagram Stories Template screens](./showcase.jpg)

## 📱 Screens (4 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Instagram Learn more 16:9** · start screen | `src/app/instagram-learn-more-16-9.jsx` | 1080 × 1920 | 1 |
| 2 | **Instagram Profile (iPhone XS)** | `src/app/instagram-profile-iphone-xs.jsx` | 375 × 812 | 2 |
| 3 | **Instagram Send message 16:9** | `src/app/instagram-send-message-16-9.jsx` | 1080 × 1920 | 2 |
| 4 | **Instagram Story 16:9** | `src/app/instagram-story-16-9.jsx` | 1080 × 1920 | 2 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Inter), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/instagram-stories-template> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **iOS Instagram Template** design by **Hugo**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Hugo](https://www.sketchappsources.com/contributor/LabelA) |
| Original design | [iOS Instagram Template](https://labela.nl/) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4089-instagram-ios-template-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/LabelA> |
| Twitter | <https://twitter.com/labela_nl> |
| Website | <http://labela.nl> |
| Original file | `instagram-template-ios-hugo.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. Instagram's name and logo are trademarks. |

**Attribution:**

> UI design: "iOS Instagram Template" by Hugo (https://labela.nl/), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4089-instagram-ios-template-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->

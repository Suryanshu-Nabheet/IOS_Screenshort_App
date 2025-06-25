# Screenshot Pro

A modern macOS application for capturing, enhancing, and saving screenshots with advanced image processing tools, built using SwiftUI and Apple’s latest frameworks.

---

## 🚀 Features

- **Full Screen & Window Capture:**  
  Capture the entire screen or a specific window using Apple’s ScreenCaptureKit for high-quality screenshots.

- **Image Enhancement Tools:**  
  - Drop shadows (customizable radius, opacity, offset)
  - Rounded corners (adjustable radius)
  - Backgrounds: solid color, gradient, or transparent
  - Padding
  - Custom text overlay (font, color, size, position, bold, italic)

- **Live Preview:**  
  Instantly see enhancements before saving.

- **SwiftUI Interface:**  
  Clean, responsive, and native macOS user experience.

- **Easy Saving:**  
  Save enhanced screenshots as PNG or JPEG using a native save dialog.

---

## 🖥️ Tech Stack

| Technology         | Purpose                                   |
|--------------------|-------------------------------------------|
| SwiftUI            | Declarative UI for macOS                  |
| AppKit             | Image processing and file dialogs         |
| ScreenCaptureKit   | High-performance screen capture           |
| Swift Concurrency  | Async/await for smooth user experience    |
| Xcode              | Apple’s IDE for macOS development         |

---

## 📁 Project Structure

```
screenshot-pro-macos-main/
│
├── screenshot/
│   ├── Assets.xcassets/             # App icons and colors
│   ├── ContentView.swift            # Main user interface
│   ├── ImageEnhancementView.swift   # Image processing/enhancement UI
│   ├── ScreenshotManager.swift      # Screenshot capture and save logic
│   ├── screenshotApp.swift          # App entry point
│   ├── screenshot.entitlements      # App sandbox and permissions
│
├── screenshotTests/
│   └── screenshotTests.swift        # Unit tests
│
├── screenshotUITests/
│   ├── screenshotUITests.swift      # UI tests
│   └── screenshotUITestsLaunchTests.swift
│
├── screenshot.xcodeproj/            # Xcode project files
└── README.md                        # Project documentation
```

---

## 📝 How It Works

1. **Capture:**  
   User selects "Full Screen" or "Window" → `ScreenshotManager` uses ScreenCaptureKit to grab the image.

2. **Enhance:**  
   Image is passed to `ImageEnhancementView` → User customizes shadow, corners, background, padding, and text overlay with live SwiftUI preview.

3. **Save:**  
   User clicks "Save" → Native dialog opens → Image is exported as PNG or JPEG.

4. **Clear:**  
   User clicks "Clear" → Current screenshot and enhancements are reset.

---

## 🔒 Permissions

- **Screen Recording:** Required for capturing screen/window content.
- **Camera & Media Library:** (Optional, for future features)

Managed via [`screenshot/screenshot.entitlements`](screenshot/screenshot.entitlements).

---

## ⚡ Requirements

- macOS 11.0 or later
- Xcode 13.0 or later

---

## 🛠️ Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Suryanshu-Nabheet/IOS_Screenshort_App.git
   ```
2. **Open the project:**
   - Open `screenshot.xcodeproj` in Xcode.
3. **Build and run:**
   - Select the `screenshot` scheme and run the app.

---

## 🤝 Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or bug fixes.

---

## 📄 License

[MIT License](LICENSE)  
(C) 2024 Suryanshu Nabheet

---

## 🙏 Acknowledgements

- Apple Developer Documentation
- SwiftUI and ScreenCaptureKit communities

---

## 📬 Contact

For questions or feedback, please open an issue

# Screenshot Pro

A modern macOS application built with SwiftUI for capturing, enhancing, and saving screenshots with advanced image processing tools.

---

## Features

- **Full Screen & Window Capture:**  
  Capture the entire screen or a specific window using Apple's ScreenCaptureKit for high-quality screenshots.

- **Image Enhancement Tools:**  
  - Add drop shadows with customizable radius, opacity, and offset.
  - Apply rounded corners with adjustable radius.
  - Set backgrounds: solid color, gradient, or transparent.
  - Add padding around screenshots.
  - Overlay custom text with configurable font, color, size, position, bold, and italic options.

- **Live Preview:**  
  Instantly see enhancements before saving.

- **SwiftUI Interface:**  
  Clean, responsive, and native macOS user experience.

- **Easy Saving:**  
  Save enhanced screenshots as PNG or JPEG using a native save dialog.

---

## Requirements

- macOS 11.0 or later
- Xcode 13.0 or later

---

## Installation

1. **Clone the repository:**
   ```sh
   git clone <repository-url>
   cd screenshot-pro-macos-main
   ```
2. **Open the project:**
   - Open `screenshot.xcodeproj` in Xcode.
3. **Build and run:**
   - Select the `screenshot` scheme and run the app.

---

## Usage

1. **Capture a Screenshot:**
   - Click "Full Screen" to capture the entire display.
   - Click "Window" to capture a specific window.

2. **Enhance the Screenshot:**
   - Click "Enhance" to open the enhancement panel.
   - Adjust shadow, corner radius, background, padding, and text overlay as desired.
   - Preview changes live.

3. **Save or Clear:**
   - Click "Save" to export the enhanced image as PNG or JPEG.
   - Click "Clear" to remove the current screenshot and start over.

---

## Project Structure

```
screenshot/
  ContentView.swift            # Main user interface
  ImageEnhancementView.swift   # Image processing/enhancement UI
  ScreenshotManager.swift      # Screenshot capture and save logic
  screenshotApp.swift          # App entry point
  screenshot.entitlements      # App sandbox and permissions
  Assets.xcassets/             # App icons and colors
screenshotTests/
  screenshotTests.swift        # Unit tests (Swift Testing framework)
screenshotUITests/
  screenshotUITests.swift      # UI tests
  screenshotUITestsLaunchTests.swift
screenshot.xcodeproj/          # Xcode project files
README.md                      # Project documentation
```

---

## Permissions

The app requests the following permissions for full functionality:

- **Screen Recording:** Required for capturing screen/window content.
- **Camera & Media Library:** (If extended) For future features or enhancements.

These are managed via the [`screenshot/screenshot.entitlements`](screenshot/screenshot.entitlements) file.

---

## Technologies Used

- **SwiftUI:** Declarative UI for macOS.
- **ScreenCaptureKit:** Modern, high-performance screen capture.
- **AppKit:** For image processing and file dialogs.
- **Swift Concurrency:** Async/await for smooth user experience.

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or bug fixes.

---

## License

[MIT License](LICENSE)  
(C) 2024 Suryanshu Nabheet

---

## Acknowledgements

- Apple Developer Documentation
- SwiftUI and ScreenCaptureKit communities

---

## Contact

For questions or feedback, please open an issue on GitHub.
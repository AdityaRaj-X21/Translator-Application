# Translator App (Hindi-English)

This Android application provides real-time translation between Hindi and English. It utilizes Google's ML Kit Translation API for accurate language translation. The app includes features like speech recognition, clipboard integration, and language swap functionality.

---

## Features

- **Real-Time Translation**: Automatically translates text entered in the input field.
- **Speech Recognition**: Convert spoken words to text and translate.
- **Language Swap**: Easily switch between translating Hindi to English and vice versa.
- **Clipboard Integration**: Copy input or translated text to the clipboard.
- **Offline Model Download**: Supports offline translation by downloading required language models.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/translator-hin-eng.git
   ```
2. Open the project in **Android Studio**.
3. Sync the project with Gradle to install dependencies.
4. Run the app on your preferred emulator or Android device.

---

## Dependencies

- **Google ML Kit Translation API**
- **Speech Recognition API**
- **Valdesekamdem MDToast Library** (for toast notifications)

Add these dependencies in your `build.gradle` file:
```gradle
implementation 'com.google.mlkit:translate:17.0.1'
implementation 'com.valdesekamdem.library:mdtoast:0.9.0'
```

---

## Usage

1. Enter text in the input field or use the microphone icon to speak.
2. Translations will automatically appear in the output field.
3. Use the **swap button** to switch translation directions.
4. Copy text using the **copy buttons**.

---

## Screenshots

_Add screenshots of your app here to visually explain its functionality._

---

## How It Works

### Translation Process:
1. The app uses `TranslatorOptions` to define language pairs:
   - English → Hindi
   - Hindi → English
2. Downloads language models using `DownloadConditions`.
3. Automatically translates text with the `Translator.translate()` method.
4. Displays translated text in the output field.

### Voice Input:
- The app integrates with `RecognizerIntent` for speech-to-text functionality.

---

## Limitations

- Requires an active internet connection for initial model downloads.
- Speech recognition accuracy depends on the device's microphone and ambient noise.

---

## Contributing

Contributions are welcome! Feel free to:
- Submit issues or feature requests.
- Fork the repository and create pull requests.

---

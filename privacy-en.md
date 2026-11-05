# Privacy Policy

**App:** Quran Muallem - معلم القرآن (Learn Quran with the help of AI), Android, iOS and web version · **Last updated:** 4 November 2026

Quran Muallem is built as a local-first app. We do not run servers for it, we do not create user accounts on any server, and we do not use analytics, advertising or tracking tools. This policy explains which data the app handles, where it is stored, and which third parties the app contacts on your behalf. It complies with the EU General Data Protection Regulation (GDPR).

## 1. Controller

Oualid Ben Rejeb
E-mail: quranmuallem@gmail.com

The app's server-free design means we (the controller) never receive your personal data. Section 4 lists the third parties that do receive data when you use certain functions.

## 2. Data stored only on your device

All data the app creates is stored **only on your device**, inside the app's private storage (Capacitor Preferences in the Android/iOS app; Local Storage, IndexedDB and Cache Storage in the web version). None of it is sent to servers operated by us. This includes:

| Data | Purpose |
|---|---|
| Profile (name, e-mail, profile picture, sign-in method) | Show your name in the app |
| Local e-mail account (e-mail and a salted PBKDF2-SHA256 **hash** of the password, never the password itself) | Protect your profile on this device |
| Memorization progress, streak, review dates, practice results (accuracy per verse) | Progress tracking and smart review |
| Settings (language, theme, reciter, speech engine, AI provider and model) | Your preferences |
| Chat history with the virtual teacher (up to 60 messages) | Show the conversation again |
| Your own AI API key (Groq or OpenAI), if you enter one | Use the virtual teacher |
| Last known position for the Qibla compass | Compass works offline |
| Cached Quran text, downloaded recitation audio, speech-recognition model files | Offline use |

**API keys:** Your key is kept in the app's private storage, which the operating system shields from other apps. The app does not apply additional encryption to it. It is sent only to the AI provider you chose (see 4.3), never to us. Do not use the app on a device that other people can unlock if you want to keep the key secret.

## 3. Speech recognition (Tasmīʿ)

When you recite, the app uses your microphone **only while recording is switched on**.

- **In the Android/iOS app:** recitation is recognised **entirely on your device** by a speech model (Whisper, via Transformers.js / ONNX Runtime using WebAssembly). The audio stays in the device's memory, is used only to compare your recitation with the Quran text, and is discarded right after. Audio is **never stored, never uploaded and never used to train AI models**. We do not use any cloud speech service.
- **Model download:** the first time you use the recognition, the model files (about 40–75 MB) are downloaded once from Hugging Face (huggingface.co) and cached on your device. No audio is sent with that request. Your IP address is visible to Hugging Face. If the model files are bundled with the app, this download does not happen.
- **Web version in a browser only:** with the speech engine set to "Automatic", the app can use your browser's built-in live speech recognition. Your browser vendor then processes the audio (for example Google in Chrome, Apple in Safari) under its own privacy terms. Choose "On-device Whisper" in Settings to avoid this.

Only the result (which words were recited correctly) is saved as part of your progress.

## 4. Third-party services the app contacts

The app connects directly from your device to the following services only when you use the related function. Each one can see your IP address and the technical data of the request, and processes it under its own privacy policy. Where these providers are located outside the EU (mostly in the USA), data is transferred to a third country. Legal basis: Art. 6(1)(b) GDPR (providing the function you requested) and Art. 6(1)(f) GDPR (our legitimate interest in providing a working app).

### 4.1 Quran text and recitation audio
- **Quran.com API** (api.quran.com) and, as a fallback, **AlQuran Cloud** (api.alquran.cloud): Quran text and surah data. The Madani Mushaf layout and Uthmani text are bundled with the app, so these are needed only rarely.
- **EveryAyah** (everyayah.com) and **mp3quran.net**: recitation audio of the 10 reciters, streamed or downloaded when you press play or download.

### 4.2 Sign-in (optional)
If you choose to sign in with **Google**, **Apple** or **Facebook**, the sign-in takes place at that provider. The app receives your user ID, name, e-mail address and profile picture **once** and stores them on your device only. The access token is not stored. Signing in "as a guest" or with a local e-mail account contacts no one.

### 4.3 Virtual teacher (AI chat, optional, Bring Your Own Key)
When you send a message to the virtual teacher, the text of your question and the recent conversation are sent **directly from your device** to the provider you selected, using **your own API key**:
- **Groq, Inc.** (api.groq.com, USA): default provider;
- **OpenAI, L.L.C.** (api.openai.com, USA): optional.

Do not enter personal or sensitive information in the chat. How long the provider keeps the data, and whether it uses it, is governed by the provider's terms (see the privacy policies of Groq and OpenAI). If the app was built with an app-wide key, your messages are sent with that key in the same way. No audio is ever sent to these providers.

### 4.4 Sharing and invitations
If you invite friends, the app opens your device's share sheet or the app/website you choose (WhatsApp, Instagram, Facebook, Telegram, X, e-mail, SMS). Only the invitation text you send is passed on.

## 5. Offline functions and location

- The **Mushaf reader** works fully offline with the bundled page data. Audio playback needs a connection unless you downloaded the recitation.
- The **Qibla compass** uses your device's GPS/location services and magnetometer. The direction and the distance to the Kaaba are **calculated on your device**. Your location is never sent anywhere and never used for tracking. The last position is saved on your device so the compass also works offline.
- Location and microphone access are requested through the operating system's permission dialog. You can revoke them at any time in your device settings (Art. 6(1)(a) GDPR).

## 6. No tracking, no ads, no profiling

The app contains no advertising, no analytics or crash-reporting SDKs, no tracking cookies and no profiling. We do not sell or share data.

## 7. Your rights and control

Because your data is on your device, you control it directly:
- **Access and export:** Settings → Progress backup → Export creates a JSON file of your progress, which you can import on another device (Art. 15 and 20 GDPR).
- **Correction:** change your name and settings in the app (Art. 16).
- **Deletion:** Settings → "Delete all my data" removes your profile, progress, chat, keys and cached files from the device. Uninstalling the app or clearing its data in the system settings has the same effect (Art. 17). Data held by the third parties in section 4 must be deleted with them directly.
- You also have the rights to restriction (Art. 18) and objection (Art. 21), and the right to **lodge a complaint with a data protection supervisory authority** (Art. 77), for example the authority of your country of residence.

For questions, contact us at quranmuallem@gmail.com. Because we hold no data about you, we usually cannot identify or retrieve your data. We can always explain how to manage it on your device.

## 8. Children

The app is suitable for learners of all ages and collects no data on our side. Children under 16 should use the sign-in options and the AI teacher only with a parent's or guardian's permission.

## 9. Changes

We will update this policy when the app's functions change. The current version is always available in the app (Settings → Legal) and via the link on the app's store page.

*If the English and Arabic versions differ, the English version prevails.*


---
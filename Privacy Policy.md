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

<div dir="rtl" lang="ar">

# سياسة الخصوصية

**التطبيق:** «Quran Muallem - معلم القرآن»، إصدار أندرويد وiOS والويب · **آخر تحديث:** ٤ نوفمبر ٢٠٢٦

صُمِّم تطبيق «Quran Muallem - معلم القرآن» ليعمل محليًا على جهازك أولًا: لا نشغّل له أي خوادم، ولا ننشئ حسابات للمستخدمين على أي خادم، ولا نستخدم أدوات تحليل أو إعلانات أو تتبّع. توضّح هذه السياسة البيانات التي يتعامل معها التطبيق، وأين تُحفَظ، والجهات الخارجية التي يتصل بها التطبيق نيابةً عنك. وهي متوافقة مع اللائحة العامة لحماية البيانات في الاتحاد الأوروبي (GDPR).

## ١. الجهة المسؤولة

Oualid Ben Rejeb
البريد الإلكتروني: quranmuallem@gmail.com

بما أن التطبيق لا يعتمد على أي خوادم، فإننا (بصفتنا الجهة المسؤولة) لا نتلقّى بياناتك الشخصية أبدًا. ويذكر البند ٤ الجهات الخارجية التي تتلقّى بيانات عند استخدامك وظائف معيّنة.

## ٢. بيانات تُحفَظ على جهازك فقط

تُحفَظ جميع البيانات التي ينشئها التطبيق **على جهازك فقط**، داخل التخزين الخاص بالتطبيق (Capacitor Preferences في تطبيق أندرويد/iOS، وLocal Storage وIndexedDB وCache Storage في إصدار الويب)، ولا يُرسَل شيء منها إلى خوادم نديرها. ويشمل ذلك:

| البيانات | الغرض |
|---|---|
| الملف الشخصي (الاسم، البريد الإلكتروني، الصورة، طريقة الدخول) | عرض اسمك في التطبيق |
| الحساب المحلي بالبريد (البريد و**قيمة تجزئة** (hash) لكلمة المرور بخوارزمية PBKDF2-SHA256 مع ملح، وليس كلمة المرور نفسها) | حماية ملفك على هذا الجهاز |
| تقدّم الحفظ، سلسلة الأيام، مواعيد المراجعة، نتائج التسميع (نسبة الدقة لكل آية) | متابعة التقدّم والمراجعة الذكية |
| الإعدادات (اللغة، المظهر، القارئ، طريقة التعرّف، مزوّد الذكاء الاصطناعي والنموذج) | تفضيلاتك |
| سجلّ المحادثة مع المعلّم الافتراضي (حتى ٦٠ رسالة) | عرض المحادثة مرة أخرى |
| مفتاح API الخاص بك (Groq أو OpenAI) إن أدخلته | استخدام المعلّم الافتراضي |
| آخر موقع معروف لبوصلة القبلة | عمل البوصلة دون إنترنت |
| نص القرآن المخزَّن مؤقتًا، والتلاوات التي نزّلتها، وملفات نموذج التعرّف على الكلام | الاستخدام دون إنترنت |

**مفاتيح API:** يُحفَظ مفتاحك في التخزين الخاص بالتطبيق الذي يحميه نظام التشغيل من التطبيقات الأخرى. لا يضيف التطبيق تشفيرًا إضافيًا للمفتاح. ولا يُرسَل المفتاح إلا إلى مزوّد الذكاء الاصطناعي الذي اخترته (انظر ٤.٣)، ولا يصل إلينا أبدًا. إن أردت إبقاء مفتاحك سرًّا، فلا تستخدم التطبيق على جهاز يستطيع غيرك فتحه.

## ٣. التعرّف على التلاوة (التسميع)

يستخدم التطبيق الميكروفون **فقط أثناء تشغيل التسجيل** عندما تتلو.

- **في تطبيق أندرويد/iOS:** يتم التعرّف على تلاوتك **بالكامل على جهازك** بواسطة نموذج كلام (Whisper عبر Transformers.js / ONNX Runtime باستخدام WebAssembly). يبقى الصوت في ذاكرة الجهاز، ويُستخدَم فقط لمقارنة تلاوتك بنص القرآن، ثم يُحذَف مباشرةً. **لا يُحفَظ الصوت ولا يُرفَع ولا يُستخدَم أبدًا لتدريب نماذج الذكاء الاصطناعي**، ولا نستخدم أي خدمة سحابية للتعرّف على الكلام.
- **تنزيل النموذج:** عند أول استخدام للتعرّف، تُنزَّل ملفات النموذج (نحو ٤٠–٧٥ ميغابايت) مرة واحدة من Hugging Face (huggingface.co) وتُخزَّن على جهازك. لا يُرسَل أي صوت مع هذا الطلب، لكن عنوان IP الخاص بك يكون مرئيًا لـ Hugging Face. وإذا كانت ملفات النموذج مضمّنة في التطبيق، فلا يحدث هذا التنزيل.
- **إصدار الويب في المتصفح فقط:** إذا كانت طريقة التعرّف «تلقائي»، فقد يستخدم التطبيق خدمة التعرّف الفوري المدمجة في متصفحك، وعندها يعالج مزوّد المتصفح الصوت وفق شروطه (مثل Google في Chrome، وApple في Safari). اختر «Whisper على الجهاز» في الإعدادات لتجنّب ذلك.

ولا يُحفَظ إلا الناتج (أي الكلمات التي تلوتها صحيحة) ضمن تقدّمك.

## ٤. خدمات خارجية يتصل بها التطبيق

يتصل التطبيق مباشرةً من جهازك بالخدمات التالية فقط عند استخدامك الوظيفة المرتبطة بها. ويمكن لكل منها رؤية عنوان IP الخاص بك والبيانات التقنية للطلب، وتعالجها وفق سياسة الخصوصية الخاصة بها. وإذا كان المزوّد خارج الاتحاد الأوروبي (غالبًا في الولايات المتحدة)، تُنقَل البيانات إلى دولة ثالثة. الأساس القانوني: المادة ٦(١)(ب) من اللائحة العامة لحماية البيانات (تقديم الوظيفة التي طلبتها)، والمادة ٦(١)(و) (مصلحتنا المشروعة في تقديم تطبيق يعمل).

### ٤.١ نص القرآن والتلاوات الصوتية
- **واجهة Quran.com** (api.quran.com)، وكبديل احتياطي **AlQuran Cloud** (api.alquran.cloud): نص القرآن وبيانات السور. ترتيب صفحات مصحف المدينة والنص العثماني مضمّنان في التطبيق، لذا لا يُحتاج إليهما إلا نادرًا.
- **EveryAyah** (everyayah.com) و**mp3quran.net**: تلاوات القرّاء العشرة، تُبَثّ أو تُنزَّل عند الضغط على التشغيل أو التنزيل.

### ٤.٢ تسجيل الدخول (اختياري)
إذا اخترت الدخول عبر **Google** أو **Apple** أو **Facebook**، يتم الدخول لدى ذلك المزوّد، ويتلقّى التطبيق معرّف المستخدم والاسم والبريد الإلكتروني والصورة **مرة واحدة** ويحفظها على جهازك فقط، ولا يُحفَظ رمز الوصول. أما الدخول «كزائر» أو بحساب بريد محلي فلا يتصل بأي جهة.

### ٤.٣ المعلّم الافتراضي (محادثة بالذكاء الاصطناعي، اختيارية، بمفتاحك الخاص)
عند إرسال رسالة إلى المعلّم الافتراضي، يُرسَل نص سؤالك وآخر المحادثة **مباشرةً من جهازك** إلى المزوّد الذي اخترته، **بمفتاح API الخاص بك**:
- **Groq, Inc.** (api.groq.com، الولايات المتحدة): المزوّد الافتراضي؛
- **OpenAI, L.L.C.** (api.openai.com، الولايات المتحدة): اختياري.

لا تُدخل معلومات شخصية أو حساسة في المحادثة. وتخضع مدة احتفاظ المزوّد بالبيانات وكيفية استخدامها لشروطه (راجع سياسات الخصوصية لدى Groq وOpenAI). وإذا بُني التطبيق بمفتاح عام مدمج، تُرسَل رسائلك بهذا المفتاح بالطريقة نفسها. ولا يُرسَل أي صوت إلى هؤلاء المزوّدين أبدًا.

### ٤.٤ المشاركة والدعوات
عند دعوة الأصدقاء، يفتح التطبيق قائمة المشاركة في جهازك أو التطبيق/الموقع الذي تختاره (واتساب، إنستغرام، فيسبوك، تيليغرام، X، البريد، الرسائل القصيرة)، ولا يُنقَل إلا نص الدعوة الذي ترسله.

## ٥. الوظائف دون إنترنت والموقع

- **قارئ المصحف** يعمل دون إنترنت بالكامل ببيانات الصفحات المضمّنة. أما الاستماع للتلاوة فيحتاج إلى اتصال ما لم تكن قد نزّلتها.
- **بوصلة القبلة** تستخدم خدمات الموقع (GPS) ومستشعر المغناطيسية في جهازك، ويُحسَب الاتجاه والمسافة إلى الكعبة **على جهازك**. لا يُرسَل موقعك إلى أي جهة ولا يُستخدَم للتتبّع أبدًا. ويُحفَظ آخر موقع على جهازك لتعمل البوصلة دون إنترنت أيضًا.
- يُطلَب إذن الموقع والميكروفون عبر نافذة الأذونات في نظام التشغيل، ويمكنك سحبه في أي وقت من إعدادات جهازك (المادة ٦(١)(أ)).

## ٦. لا تتبّع ولا إعلانات ولا تنميط

لا يحتوي التطبيق على إعلانات، ولا على أدوات تحليل أو تقارير أعطال، ولا على ملفات تعريف ارتباط للتتبّع، ولا يقوم بأي تنميط. ولا نبيع البيانات ولا نشاركها.

## ٧. حقوقك وتحكّمك

بما أن بياناتك على جهازك، فأنت تتحكّم بها مباشرةً:
- **الاطّلاع والتصدير:** الإعدادات ← النسخ الاحتياطي للتقدّم ← تصدير، ينشئ ملف JSON بتقدّمك يمكنك استيراده على جهاز آخر (المادتان ١٥ و٢٠).
- **التصحيح:** غيّر اسمك وإعداداتك داخل التطبيق (المادة ١٦).
- **الحذف:** الإعدادات ← «حذف جميع بياناتي» يزيل ملفك وتقدّمك والمحادثة والمفاتيح والملفات المخزّنة من الجهاز، وكذلك حذف التطبيق أو مسح بياناته من إعدادات النظام (المادة ١٧). أما البيانات لدى الجهات الخارجية في البند ٤ فيجب طلب حذفها منها مباشرةً.
- لك أيضًا حق تقييد المعالجة (المادة ١٨) والاعتراض (المادة ٢١)، و**حق تقديم شكوى إلى سلطة رقابية لحماية البيانات** (المادة ٧٧)، مثل السلطة في بلد إقامتك.

للاستفسارات راسلنا على quranmuallem@gmail.com. وبما أننا لا نحتفظ بأي بيانات عنك، فلا نستطيع عادةً تحديد بياناتك أو استرجاعها، لكننا نشرح لك دائمًا كيف تديرها على جهازك.

## ٨. الأطفال

التطبيق مناسب للمتعلّمين من جميع الأعمار، ولا نجمع أي بيانات من جهتنا. ويُستحسَن أن يستخدم الأطفال دون ١٦ عامًا خيارات تسجيل الدخول والمعلّم الافتراضي بإذن وليّ الأمر.

## ٩. التغييرات

سنحدّث هذه السياسة عند تغيّر وظائف التطبيق. وتتوفّر النسخة الحالية دائمًا داخل التطبيق (الإعدادات ← المعلومات القانونية) وعبر الرابط في صفحة التطبيق في المتجر.

*في حال وجود اختلاف بين النسختين العربية والإنجليزية، تُعتمَد النسخة الإنجليزية.*


</div>

---
AVANISH LUDO ANDROID APP
=========================

यह Android Studio project है।

IMPORTANT:
यह project online Ludo game को Android APK के अंदर चलाता है।
Multiplayer server अलग से Internet पर deploy करना जरूरी है।

STEP 1 - SERVER:
अपने Node.js/Socket.IO Ludo server को Render या किसी दूसरे Node.js
hosting provider पर deploy करें।

उदाहरण:
https://avanish-ludo-online.onrender.com

STEP 2 - APP URL:
इस file को खोलें:

app/src/main/java/com/avanish/ludo/MainActivity.java

यह line खोजें:

private static final String GAME_URL =
        "https://YOUR-SERVER-URL.onrender.com";

इसे अपने असली server URL से बदलें।

STEP 3 - ANDROID STUDIO:
1. Android Studio install करें।
2. Open चुनें और यह पूरा folder खोलें।
3. Gradle sync पूरा होने दें।
4. Run दबाकर मोबाइल/Emulator पर test करें।

STEP 4 - APK:
Android Studio में:
Build -> Build Bundle(s) / APK(s) -> Build APK(s)

फिर APK install करके test करें।

IMPORTANT:
- Server URL HTTPS होना चाहिए।
- Socket.IO server उसी URL/domain पर उपलब्ध होना चाहिए।
- यह WebView wrapper है; Ludo game का realtime logic server/web app में रहता है।
- Production app के लिए app icon, splash screen, login, reconnect,
  notifications, matchmaking, database और anti-cheat बाद में जोड़े जा सकते हैं।

# Habs – build the Android APK

Needs: Node.js 20+, Android Studio (includes the SDK and JDK).

1. npm install
2. npx cap add android
3. npx cap sync
4. npx cap open android
5. In Android Studio wait for Gradle to finish, then
   Build > Build Bundle(s) / APK(s) > Build APK(s)
6. Click "locate" in the popup. app-debug.apk is in
   android/app/build/outputs/apk/debug/
7. Copy the APK to your phone and install it
   (allow "Install unknown apps" when asked).

To change the app later: edit www/index.html, then run
npx cap sync and rebuild.

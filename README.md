# Rede Cloud Android APK

Android WebView shell for Rede Cloud v19.

## Default server
`http://192.168.11.229:2027`

The app includes a **Ganti Server** menu so the URL can be changed later (for example to a domain or Cloudflare URL). The selected URL is saved on the device.

## Included Android features
- Rede Cloud icon/branding
- WebView with JavaScript and local storage
- File picker for uploads
- Android DownloadManager for downloads
- Back button navigation
- Cleartext HTTP support for local server usage
- Server URL configuration
- Responsive Rede Cloud web UI

## Build with Android Studio
1. Open this folder in Android Studio.
2. Let Gradle download Android Gradle Plugin 8.7.2 and compile SDK 35.
3. Build > Generate App Bundle / APK > Generate APK.
4. The debug APK will normally be under `app/build/outputs/apk/debug/app-debug.apk`.

## Important
The APK is a client for the Docker Rede Cloud server; it does not contain the PostgreSQL database or user files. The server must be reachable from the Android device.

For your current LAN setup, the default URL is `http://192.168.11.229:2027`. If the phone is on another network, use **Ganti Server** and enter the reachable HTTPS/domain URL.

# La Persona — Black Edition Live Wallpaper

This is a **real Android Studio project** implementing a silent looping live wallpaper via WallpaperService + MediaPlayer, plus the 15-second MP4 preview. It is **not an APK yet**: open the project in Android Studio on Windows, allow Gradle to sync, choose Build > Build APK(s), and install the generated APK on your Samsung phone. Open the app and tap Preview & set live wallpaper. Requires Android 8.0+.

The project is a first functional version, not the full Samsung One UI theme, keyboard, or parallax 3D engine. The wallpaper uses subtle animated movement over the supplied artwork and is silent. Video playback can use more battery than a static wallpaper. Test on device before publishing.


## Tilt-responsive version
This build uses the phone's rotation-vector sensor to move the wallpaper in response to tilting. It smoothly eases movement, clamps it to ~3.4% of screen width, and draws a subtle animated ember layer. The original video is kept as an asset but the live wallpaper now renders a still image with parallax and embers (the video itself is not playing). It pauses sensor readings and rendering when hidden. No special sensor permissions required. The app must be built with Android Studio; no APK included. Test on physical Samsung hardware, since this code has not been device-tested.

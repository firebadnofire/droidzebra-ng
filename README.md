# DroidZebra (Android)

DroidZebra is a graphical front-end for the Zebra Othello/Reversi engine by Gunnar Andersson. This repository is a fork of the original GPLv3 project:

- Upstream source: https://github.com/alkom/droidzebra

All new contributions in this fork are released under the same GPLv3 license as the original project.

## Android Studio (Gradle)

This repository includes a modern Gradle setup so the root folder can be opened directly in Android Studio.

1. Open Android Studio and choose **Open** on the repository root.
2. Ensure the Android NDK is installed (the build uses ndk-build).
3. Set the project SDK to Android 16 (API 35) or higher when prompted.

The Gradle `app` module points to the legacy `project/` sources and JNI build files, keeping the original layout intact while supporting modern Android toolchains.

## Project layout

- `project/` — legacy Android project (Java, resources, manifest, JNI).
- `app/` — Gradle wrapper module that references the legacy sources.
- `Application.mk` — top-level NDK configuration.

## License

GPLv3. See `old.README.md` for the original project notes and history.

# Mojo Glow Worm

A performance-focused Minecraft: Java Edition launcher for Android, based on [MojoLauncher](https://github.com/MojoLauncher/MojoLauncher) and [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher).

Designed for low-end Android devices with optimization and lightweight resource usage in mind.

## Overview

Mojo Glow Worm is a customized fork of MojoLauncher tailored for:

- **Low-end Android devices** — optimized for older and resource-constrained phones
- **Performance** — focused on smooth gameplay with minimal resource overhead
- **Stability** — reliable Minecraft: Java Edition launcher experience
- **Familiar interface** — maintains the MojoLauncher-style user experience

## Features

- **Minecraft Java Edition Support** — Play most Minecraft versions on Android
- **Modding Support** — Forge and Fabric modloader support
- **Modpack Import** — Import CurseForge and mrpack modpacks
- **Instance System** — Manage multiple game instances/profiles
- **Multi-version Support** — From classic versions to latest snapshots
- **Low-end Optimization** — Tuned for budget Android devices

## Minecraft Version Support

Supports a wide range of Minecraft: Java Edition versions, including:

- Classic and early versions
- All release versions up to latest
- Snapshots and pre-releases
- Combat Test versions

*Version support depends on the underlying PojavLauncher runtime.*

## Modding

Fully compatible with:

- **Forge** — Use Forge installers to install Forge modloaders
- **Fabric** — Install and use Fabric mods
- **Modpacks** — Import CurseForge and mrpack format modpacks

## Android Compatibility

- **Minimum Android**: API 21 (Android 5.0 Lollipop)
- **Target Android**: API 36 (Android 15)
- **Architecture**: Multiarch support (arm64-v8a, armeabi-v7a, x86, x86_64)
- **Java**: Java 1.8 compatibility

## Building from Source

### Requirements

- JDK 8 or higher
- Gradle (included via gradlew)
- Android NDK 29.0.14206865
- Android SDK (API level 36)

### Build Command

```bash
./gradlew :app_pojavlauncher:assembleDebug
```

On Windows, use:

```bash
.\gradlew.bat :app_pojavlauncher:assembleDebug
```

### Build Variants

- **full** — Includes embedded JRE 8 (larger APK, ready to use)
- **noruntime** — Without embedded runtime (requires separate installation)

### Output APK

The compiled APK will be at:

```
app_pojavlauncher/build/outputs/apk/full/debug/app_pojavlauncher-full-debug.apk
```

or

```
app_pojavlauncher/build/outputs/apk/noruntime/debug/app_pojavlauncher-noruntime-debug.apk
```

## Installation

1. **Build or obtain the APK** (see Building section above)
2. **Enable installation from unknown sources** on your Android device
3. **Transfer the APK** to your device
4. **Install** by tapping the APK file
5. **Launch** Mojo Glow Worm and enjoy Minecraft

## Getting Prebuilt APKs

- **GitHub Releases** — Check the [releases page](https://github.com/kings880/MojoLauncher/releases) for prebuilt APKs
- **GitHub Actions** — Early/development builds available from [Actions](https://github.com/kings880/MojoLauncher/actions)
- **Google Play** — Available on Google Play Store (see original MojoLauncher)

## Development

To contribute to Mojo Glow Worm:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test by building the debug APK
5. Submit a pull request with a clear description of your changes

## Project Status

Active development. This is a performance-optimized fork of MojoLauncher with ongoing improvements for low-end device support.

## Roadmap

### Completed

- [x] Instance system for profile management
- [x] Support for Minecraft 1.21.5
- [x] CurseForge/mrpack modpack import
- [x] Multi-version launcher functionality

### Planned

- [ ] Further low-end device optimization
- [ ] Compute shader support improvements
- [ ] Modpack/mod management tools
- [ ] MMC-compatible instance import
- [ ] Performance profiling and tuning

## Known Issues

- Some physical mice may exhibit slow cursor speed
- Large texture atlases on older GL implementations may appear distorted
- Performance varies by device capability

For detailed issues, check the [issue tracker](https://github.com/kings880/MojoLauncher/issues).

## License

This project is licensed under [GNU Lesser General Public License v3.0](./LICENSE).

Mojo Glow Worm is based on open-source projects and maintains their licensing requirements.

## Credits & Upstream Projects

- **[MojoLauncher](https://github.com/MojoLauncher/MojoLauncher)** — Base launcher project ([GNU LGPLv3](https://github.com/MojoLauncher/MojoLauncher/blob/v3_openjdk/LICENSE))
- **[PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher)** — Original launcher foundation ([GNU LGPLv3](https://github.com/PojavLauncherTeam/PojavLauncher/blob/v3_openjdk/LICENSE))
- **[OpenJDK](https://github.com/PojavLauncherTeam/openjdk-multiarch-jdk8u)** — Java runtime ([GNU GPLv2](https://openjdk.java.net/legal/gplv2+ce.html))
- **[Holy GL4ES](https://github.com/artdeell/gl4es_extra_extra/)** — Graphics library ([MIT License](https://github.com/ptitSeb/gl4es/blob/master/LICENSE))
- **[GLFW](https://github.com/MojoLauncher/glfw)** — Window management ([zlib license](https://github.com/MojoLauncher/glfw/blob/glfw34/LICENSE.md))
- **[SDL](https://github.com/MojoLauncher/MojoSDL)** — Input handling ([zlib license](https://github.com/MojoLauncher/MojoSDL/blob/main/LICENSE.txt))
- **[LWJGL](https://github.com/LWJGL/lwjgl3)** — Java bindings ([BSD-3 License](https://github.com/LWJGL/lwjgl3/blob/master/LICENSE.md))
- **[Mesa 3D](https://gitlab.freedesktop.org/mesa/mesa)** — Graphics library ([MIT License](https://docs.mesa3d.org/license.html))
- **Android libraries** — Various Apache 2.0 licensed components

## Contributing

Contributions are welcome! Please:

1. Describe your changes clearly in pull request descriptions
2. Test your changes before submitting
3. Follow existing code style conventions
4. Reference any related issues

## Support

For issues, feature requests, or questions:

- Open an [issue](https://github.com/kings880/MojoLauncher/issues) on GitHub
- Check existing issues for similar problems
- Provide detailed device and version information with bug reports

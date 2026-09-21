# PocketBuild Runtime

This repository publishes the optional Android-native runtime used by PocketBuild's **Install offline runtime** button. It contains build tooling only; PocketBuild projects remain local and never require GitHub.

The initial target is `arm64-v8a`. The runtime is built for PocketBuild's app-specific prefix and must not contain stock Termux packages.

The GitHub Actions workflow builds the execution base first. It is intentionally not a release until Java 21, Android SDK/build tools, CMake, NDK r29, and Git have been built and tested together.

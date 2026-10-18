# Magnet Clash

An Android version of the magnetic stone table-top game.

## How to play

- The 24 magnets are divided evenly among the players.
- Take turns dropping one magnet inside the flower ring (touch, drag to aim, let go).
- Magnets that are too close pull each other in. If any magnets snap together on your turn, you take all of them back.
- The first player to place all of their magnets wins.

Modes: 1 player vs computer, or 2–4 players pass-and-play.

## Get the APK

Every push runs the **Build** workflow. Open the **Actions** tab, pick the latest run and download
`magnet-clash-apk` under **Artifacts**. Unzip it and install `app-debug.apk` on your phone
(allow "Install unknown apps" when asked).

## Build locally

Open the project in Android Studio and press Run, or:

```
./gradlew assembleDebug        # APK in app/build/outputs/apk/debug/
./gradlew testDebugUnitTest    # physics and rules tests
```

## Code

- `MagnetWorld.kt` – magnet physics and the computer opponent
- `Game.kt` – turns and rules
- `GameView.kt` – drawing, touch input and animations
- `MainActivity.kt` – menu

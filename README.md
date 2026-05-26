# WGRALGO Who Said It? — Knowledge Is the Weapon Edition

Who Said It? — Knowledge Is the Weapon™ Edition is a free educational Android app from The Wealth Gap Resolution Algorithm™ Inc. It helps users practice quote recognition, wisdom categories, critical thinking, and attribution awareness through randomized 10-round quiz gameplay.

The app is fully offline, contains no ads, no analytics, no trackers, and asks for **no** Android permissions — `INTERNET` is intentionally not declared.

---

## Features

- 80+ built-in, attribution-checked quote questions across 14 wisdom categories
- Randomized 10-question rounds with multiple-choice gameplay
- Real-time score, progress bar, and per-question difficulty + category badges
- Instant feedback with the real speaker and a short explanation of each quote
- Final results screen with rating tier and Play Again
- Premium WGRALGO black-and-gold design language
- Phone and tablet responsive layout
- Fully offline: no internet permission, no network calls
- No accounts, no ads, no analytics, no trackers
- GPLv3 licensed

## Wisdom categories

Knowledge · Education · Power · Freedom · Courage · Justice · Leadership · Money and Work · Critical Thinking · Creativity · Discipline · Community · History · Technology and Change

## Screenshots

Screenshots of the home, how-it-works, question, feedback, and results screens are in [`/screenshots`](./screenshots).

## How to install / sideload the APK

1. Download `WhoSaidIt-v1.0.0.apk` from the [GitHub Releases](../../releases) page.
2. On your Android device, allow installs from your browser or file manager (Settings → Apps → Special access → Install unknown apps).
3. Open the downloaded APK and tap **Install**.
4. Optional integrity check (Linux/macOS):
   ```bash
   sha256sum WhoSaidIt-v1.0.0.apk
   ```
   Compare the output with `WhoSaidIt-v1.0.0.apk.sha256` from the same release.

## How to build from source

Requires Node.js 18+, Java 17, and the Android SDK.

```bash
git clone https://github.com/WGRALGO/WGRALGO-Who-Said-It.git
cd WGRALGO-Who-Said-It
npm install
npx cap sync android
cd android
./gradlew assembleDebug
```

The debug APK lands at `android/app/build/outputs/apk/debug/app-debug.apk`.

### Signed release build

Release signing uses `android/keystore.properties` **or** environment variables (`WSI_KEYSTORE_FILE`, `WSI_KEYSTORE_PASSWORD`, `WSI_KEY_ALIAS`, `WSI_KEY_PASSWORD`). The keystore and its passwords are **never** committed to git.

```bash
npx cap sync android
cd android
./gradlew assembleRelease
```

Output: `android/app/build/outputs/apk/release/app-release.apk`.

## Privacy summary

- No account required
- No ads
- No analytics
- No trackers
- No cloud upload
- No data selling
- No personal data is collected
- No answers or scores are sent to WGRALGO
- The app is an offline educational quote-recognition game

Full statement: [PRIVACY.md](./PRIVACY.md).

## Educational disclaimer

Who Said It? — Knowledge Is the Weapon™ Edition is for educational awareness and entertainment only. Quote attributions should be treated carefully, and users should verify important quote history through trusted sources. The app does not provide legal, financial, medical, academic, or professional advice.

## Quote attribution note

Quote attributions are drawn from widely-cited public records (primary sources, published speeches, well-documented letters, and major scholarly references). Where attribution is contested, the in-app explanation credits the popularizer and flags the dispute (for example, the "survival of the most adaptable" quote is attributed to Leon C. Megginson, not Darwin; the "we are what we repeatedly do" formulation is attributed to Will Durant, not Aristotle directly).

If you find an attribution error, please open an issue on this repository with a primary-source citation and we will fix it in the next release.

## License

This project is released under the GNU General Public License v3.0. See [LICENSE](./LICENSE).

## Contributors

See [CONTRIBUTORS.md](./CONTRIBUTORS.md).

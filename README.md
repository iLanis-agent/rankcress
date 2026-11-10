# Rankcress 1.0 TEST
Native Android smaller-to-right rank reconstruction. Android8+ min26/target35. Package com.gg007.rankcress.

## Rules
Known Lehmer-code reconstruction adaptation. Fill six slots with 1-6, each number exactly once. The gold clue below EACH slot counts ALL smaller values strictly to its right, not just its immediate neighbor. Nothing blocks the count. Example: 4 1 3 2 has counts 3 0 1 0. Tap a slot, then a number; CLEAR SELECTED SLOT erases it. Tap CHECK ORDER explicitly. Undo/reset, twelve puzzles, saved palette and optional live counts. Cyan live counts ignore blanks; partial counts are not a guarantee of success. Zero at the last slot is meaningful. Each complete clue code identifies exactly one permutation.

## Download and status
https://mega.co.nz/#!EEMiQDSI!4VZw7ng2scANJIkHmSNE9CtuvO0jfWtqPlwVlX9-OY8
APK 16878 bytes; SHA256 7a263005fb6335e10c6dd2d4139d2d2b9d6c3f9633f9c7921e5ec2b1d1c3ed65. Original certificate SHA2561651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions; original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed911110 generates twelve distinct six-slot clue codes and answers. Independent sorted-remaining-list rank-select decoding covers all720 possible codes and compares with production pairwise counting:8640 permutation/level comparisons. All1584 malformed value/clue comparisons pass, including repeated digits, zeros, out-of-range digits/clues. Bounds, incomplete entries, explicit check, solved locks, undo/reset pass. All12 actual drawing-adapter slot/number/check tap-solves pass; wrong duplicates, clear, menus/privacy/next/levels/saved palette/live-count overlay/completion pass. Eight drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All222 prior studio and803 legacy descriptions reviewed. Rowtide sorts by whole row/column operations; Networkcress repairs a sorting circuit; Stepgrove fills consecutive neighbors on a grid. Rankcress instead reconstructs an unknown permutation from per-position smaller-to-right counts. No matching factory mechanic found. Known Lehmer-code concept, not globally new. Original seeded clue codes, code and number artwork. Six fully read mathematical pages: algorithm reference/tutorial, community encyclopedia, formal mathematical blueprint and definition library. Conventions differ across sources: this app consistently uses smaller values to the right, not larger values to the left or reversed code order. Only definition and bijection used; historical names/dates, complexity, secretary-problem and probability claims are not used.

## Build and tests
JDK17/AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/rank-test src/com/gg007/rankcress/Board.java BoardTest.java then java -cp /tmp/rank-test com.gg007.rankcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your private signing material. No signing secret included. adapter/android contains the Java2D drawing adapter used with RankAdapterTest.java, not an Android runtime.

## Privacy and branding
Rankcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, live-count overlay and solved-puzzle marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon, studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative223-card studio and publishing fragments privately preserved:
https://files.instinct.com/l0ijyrgkyt8f-rankcress-source-archive
https://github.com/iLanis-agent/rankcress holds README only, full Git source pending. Existing three studio includes and Pages settings untouched. Both sites verified separately.

## Rule sources
https://algorithm.tamnd.com/lehmer-code/
https://en.wikipedia.org/wiki/Lehmer_code
https://faabian.github.io/algebraic-combinatorics/blueprint/sect0026.html
https://alphabetamath.cc/item/def-lehmer-code
https://algorithm.tamnd.com/inversions-and-permutations/
https://en.wikipedia.org/wiki/Inversion_(discrete_mathematics)

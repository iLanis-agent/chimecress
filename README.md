# Chimecress 1.0 TEST
Native Android Kin-Kon-Kan mirror-placement puzzle. Android 8+ (min26), target35. Package com.gg007.chimecress. Twelve original unique boards on a 4x3 grid.

## Rules
Kin-Kon-Kan on a 4x3 grid. Place exactly one slash or backslash mirror in every outlined room. A labeled beam enters perpendicular to the frame, travels straight through room borders and turns 90 degrees at each mirror. It must exit at the matching letter after exactly the printed number of reflections. Every mirror must reflect at least one labeled beam. Rays may cross empty cells or share mirrors; every encounter counts, including repeated mirrors. Tap a cell to cycle empty, slash, backslash, empty. Twelve original uniquely solved room layouts and twelve different mirror placements; undo/reset, levels and saved palette/beam overlay. Known Kin-Kon-Kan adaptation.

## Download and status
https://mega.co.nz/#!dcVFmCRB!g3ulRza_eH1Jw6QsrIL0eWFB3CQnyqUki0IBMdms9cc
APK SHA256 a36dd9bcaae3e5c71e1793b39a78350aed001185f661c5cee8259d6d9ab0f937; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Portable seed-801110 generator enumerates all 1,296 one-mirror-per-room choices for each original four-room layout. Twelve distinct uniquely solved room layouts and mirror placements. Every mirror is used, and every board has a beam with two or more reflections. Independent oracle builds an undirected half-edge optical graph and walks components; production steps through coordinates with direction-state cycle detection. All 6,377,292 complete ternary mirror states plus 120,000 randomized/invalid mirror masks agree. Bounds, undo/replay/reset and solved lock pass. Actual drawing-adapter cell-center taps solve all twelve and check menu, privacy, levels, next and saved palette/beam-overlay/completion. Seven drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 211 live studio descriptions and all 803 legacy entries. No paired-edge ray and room-quota mirror-placement match found. Prism Relay rotates provided mirrors to visit ordered relays and one receiver; Chimecress chooses both location and orientation, one mirror per room, for multiple paired rays with exact reflection counts and every mirror used. Mistcress places monsters around fixed mirrors; Reflectcress draws a single loop through fixed triangle reflectors. Legacy BankShot computes one-cushion pool geometry, not mirror placements. Known Kin-Kon-Kan adaptation; original generated layouts, code and visuals, not a globally new interaction. Six sources span official Japanese Nikoli rules, independent multilingual rules, a constructor tutorial, a solver reference, a playable implementation and a mobile developer listing. No source layouts, code or art copied.
Rules https://www.nikoli.co.jp/ja/puzzles/kinkonkan/ ; independent rules https://www.keepitsimplepuzzles.com/how-to-solve-a-kin-kon-kan-puzzle/ .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/chimecress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.chimecress.ChimeBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Chimecress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, optional beam overlay and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 212-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/qyknb4lrm6a2-chimecress-source-archive . Repository https://github.com/iLanis-agent/chimecress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.

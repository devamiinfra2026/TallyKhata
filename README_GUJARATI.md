# TallyKhata Android Studio Project

આ Android Studio માં ખોલી શકાય તેવો પ્રારંભિક Android project છે. તેમાં હાલની Gujarati/Hindi/English TallyKhata વેબ એપ Android WebView ની અંદર ચાલે છે.

## Project ખોલવાની રીત
1. કમ્પ્યુટરમાં Android Studio ઇન્સ્ટોલ કરો.
2. આ ZIP extract કરો.
3. Android Studio માં **Open** પસંદ કરીને `TallyKhata_Android` ફોલ્ડર પસંદ કરો.
4. Gradle Sync પૂર્ણ થવા દો. Android SDK Platform 36 અને JDK 17 ઇન્સ્ટોલ હોવા જોઈએ.
5. Android ફોનમાં Developer options અને USB debugging ચાલુ કરીને ફોન જોડો.
6. Android Studio માં Run દબાવીને વાસ્તવિક ફોન પર પરીક્ષણ કરો.

## મહત્વની મર્યાદાઓ — હજી Play Store માટે તૈયાર નથી
- આ source project છે; APK અથવા signed AAB તૈયાર થયેલી નથી.
- હજી વાસ્તવિક ફોન પર build/run અને સંપૂર્ણ QA કરવાનું બાકી છે.
- હાલનો ડેટા WebView localStorage માં રહે છે; uninstall/clear data થી ગુમાઈ શકે છે. Backup વારંવાર લો.
- હાલ PIN માત્ર સ્થાનિક convenience lock છે; encryption અથવા cloud account નથી.
- Premium billing, cloud sync, multi-device sync અને server backup અમલમાં નથી.
- Privacy Policy, Data Safety, Play Store screenshots/listing, signing key અને Play review તૈયાર કરવાના બાકી છે.
- કોઈપણ વાસ્તવિક ગ્રાહકના હિસાબથી પહેલાં test data વડે જ તપાસો.

## Signed AAB બનાવવાની રીત (પરીક્ષણ પછી)
Android Studio → Build → Generate Signed Bundle / APK → Android App Bundle → Create new keystore → Release → Finish.
Keystore અને passwords સુરક્ષિત રાખો; તેને કોઈને મોકલશો નહીં. આ AAB ને સીધી Play Console માં મૂકતાં પહેલાં તમામ પરીક્ષણ અને Play Console વિગતો પૂર્ણ કરવી જરૂરી છે.

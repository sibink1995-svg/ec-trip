# Trip Kanakku – APK build (GitHub Actions)

1. GitHub-ൽ പുതിയ repository ഉണ്ടാക്കുക (private ആയാലും മതി).
2. ഈ zip-ലെ എല്ലാ ഫയലുകളും repository-യിലേക്ക് upload ചെയ്യുക
   (www ഫോൾഡർ, package.json, capacitor.config.json, .gitignore, .github ഫോൾഡർ).
   - .github ഫോൾഡർ upload-ൽ വിട്ടുപോയാൽ: Add file > Create new file ->
     പേരായി  .github/workflows/build-apk.yml  എന്ന് ടൈപ്പ് ചെയ്ത്
     ഫയലിലെ ഉള്ളടക്കം paste ചെയ്യുക.
3. Actions ടാബ് > "Build APK" > Run workflow (main-ലേക്ക് push ചെയ്താലും തനിയെ തുടങ്ങും).
4. 5-10 മിനിറ്റിൽ കഴിയും. അവസാനിച്ച run തുറന്ന് താഴെ Artifacts-ലെ
   trip-kanakku-apk ഡൗൺലോഡ് ചെയ്യുക > zip extract ചെയ്യുക > app-debug.apk.
5. ഫോണിൽ install ചെയ്യുക (Unknown sources അനുവദിക്കണം).

ശ്രദ്ധിക്കാൻ:
- ഇത് debug APK ആണ്; സ്വന്തം ഉപയോഗത്തിന് മതി. Play Store-ന് signed release build വേണം.
- ഡാറ്റ ഫോണിൽ മാത്രം സേവ് ആകും. ആപ്പ് uninstall ചെയ്താൽ മായും.
- PDF ബട്ടൺ share sheet തുറക്കും; അതിൽ നിന്ന് Files-ൽ സേവ് ചെയ്യാം, WhatsApp-ൽ അയക്കാം.

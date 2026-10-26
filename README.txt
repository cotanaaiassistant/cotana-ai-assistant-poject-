FRIEND COTANA v17 — OFFICIAL WEBSITE

WHAT WORKS
- Fully responsive static website, animated hero, navigation
- Sinhala / English switch
- Install guide tabs (Setup.exe and Python)
- Copy-to-clipboard commands
- FAQ accordion
- Download button automatically becomes active when you set RELEASE_URL
- Privacy and release status notes
- Local logo included, no web framework or paid hosting required

PUBLISH
1. Open index.html locally to preview.
2. Test your Windows installer on another Windows computer.
3. Upload installer to GitHub Releases (or another trusted HTTPS host).
4. Open index.html in Notepad and replace:
     const RELEASE_URL = "";
   with:
     const RELEASE_URL = "https://github.com/YOUR_USERNAME/YOUR_REPO/releases/download/v17.1/Friend_Cotana_Setup_v17_1.exe";
   Use the ACTUAL URL of the tested release; do not invent one.
5. Upload index.html and the entire assets folder to a GitHub Pages repository.
6. Repository Settings > Pages > Deploy from a branch > main / (root).
7. Visit the resulting site URL and test buttons, language, and download.

SECURITY AND PRIVACY
- Never upload API keys, tokens, personal files, or user profile data.
- Installer must include the dist _internal folder, not the build folder.
- Unsigned Windows EXEs may show warnings; do not tell users to bypass security without verifying the binary.
- Publish a complete privacy policy describing microphone, Google speech services, gTTS, Ollama, and WhatsApp integrations before broad release.
- Static website works without a backend; the download requires an actual hosted installer.

FILES
index.html
assets/friend-cotana.png
README.txt

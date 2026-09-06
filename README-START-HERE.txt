ForgeAPK Studio — Fresh v5

Suggested new repository name:
ForgeAPK-Studio

Included:
- Premium redesigned builder UI
- Camera / microphone / location / notifications
- Files / gallery / audio / video
- Share / haptics / device / network
- Background Audio option
- Foreground Android media service for music playback
- Playback can continue while minimized/screen locked
- Hardware acceleration + large heap
- Medium-level web/media/3D apps
- ~90 MB source ZIP target
- 45 minute build timeout
- Old APK removed from current downloads/ when a new build succeeds
- Successful jobs/<build-id>.zip removed

Background audio JS API in generated apps:
NativeBridge.bgAudioPlay(url, "Song title")
NativeBridge.bgAudioPause()
NativeBridge.bgAudioResume()
NativeBridge.bgAudioStop()

Important:
A full MX Player-class app with custom codecs, DRM, casting and advanced subtitle engines still needs more native Android code.
This fresh version is for medium-level apps and personal use.

Setup:
1. Create a new PUBLIC GitHub repository named ForgeAPK-Studio
2. Upload index.html
3. Create .github/workflows/build-apk.yml and paste the included workflow
4. Settings > Pages > Deploy from branch > main > /(root)
5. Edit your fine-grained token:
   - give access to ForgeAPK-Studio
   - Contents: Read and write
   - Actions: Read and write
6. After the new repo works, remove the old two repos from that token if you want.

Never send your GitHub token in chat.

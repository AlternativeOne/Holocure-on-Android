# Holocure-on-Android

Big thanks to u/Capercailie [https://www.reddit.com/user/Capercailie/] for his/her work on the topic [https://www.reddit.com/r/holocure/comments/vrjwia/a_barely_working_attempt_at_an_unofficial/].

If you are here for apk - just download from the latest release on "Releases" page.

Instruction:

0. This was done on Ubuntu 20.04 so all the instruction are for this OS.
1. Install GameMaker Beta for Linux (all steps were done with GameMaker Beta 2023.100.0.273)
2. Place runtime-2023.800.0.410 folder from Runtime folder into /home/USER_NAME/.local/share/GameMakerStudio2-Beta/Cache/runtimes (or actual path of runtime if your GameMaker uses any other one)
3. Change runtime in GameMaker to runtime-2023.800.0.410
4. Open HolocureAndroid project in Project folder
5. Compile app for Android (DO NOT change targetSdk var in project settings as it will cause unfixable bug when starting a run)
6. Unzip apk that you got
7. Change assets folder with assets folder from Assets
8. Zip your apk without compression (zip -0 -r holocure.apk *)
9. zipallign your apk (zipalign -p 4 holocure.apk holocure_aligned.apk)
10. Sign your apk using apksigner tool from android-sdk (apksigner sign --ks PATH_TO_YOUR_KEYSTORE holocure_aligned.apk)
11. ???
12. Profit!


I am not affiliated with Hololive, Cover Corp., Holocure Team or GameMaker. All trademarks are proterty of their owners. This is unofficial project.

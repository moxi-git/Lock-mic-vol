# Lock-mic-vol

### what it does?
This simple set of files addresses an issue with Windows mic volume auto-controlling. because it can be anoying when your playing a game with friends and it suddenly drops to 20% or smth like that

### Instructions

1. Download these files https://github.com/moxi-git/Lock-mic-vol/releases/download/idk/Lock.mic.vol.zip

2. Extract the files

3. In the file "lock_mic_vol.bat" the default value is "58321" which is 89%, so if you want to make the volume lock onto 50% then just do some simple math ((65536/100)*50) which will give you 32768, so replace "58321" with "32768" to make the volume level lock onto 50

4. Go to the directory "C:\Windows" and paste the files : " hide_cmd_window2.vbs, lock_mic_vol.bat, nircmdc.exe "

5. Then you can run the file "start_lock_mic_vol.bat". (If you want to make this run automatically at startup then paste this file in the directory "C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp", this will automatically run the script on startup)

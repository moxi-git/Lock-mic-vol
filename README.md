# Lock-mic-vol

### What does it do?

This simple set of files fixes an issue where Windows automatically changes your microphone volume.
It can be annoying when you’re playing a game with friends and your mic suddenly drops to 20% or something like that.

---

### Instructions

1. **Download** the files: https://github.com/moxi-git/Lock-mic-vol/releases/download/idk/Lock.mic.vol.zip
   
   you can also download [pyvol_calc](https://github.com/moxi-git/Lock-mic-vol/releases/download/idk/pyvol_calc.exe) to help you calculate the volume

3. **Extract** the files.

4. **Edit the mic volume lock value**:

   * In `lock_mic_vol.bat`, the default value is `58321` (which equals 89%).
   * If you want to lock it to 50%, do the math (65536 is 100% btw):

     ```
     (65536 / 100) * 50 = 32768
     ```

     Replace `58321` with `32768` in the script.

5. **Copy the following files to** `C:\Windows`:

   ```
     hide_cmd_window2.vbs
     lock_mic_vol.bat
     nircmdc.exe
     start_lock_mic_vol.bat
   ```

6. **Run the script**:
   * To make it run automatically at startup, copy **hide_cmd_window2.vbs, lock_mic_vol.bat, nircmdc.exe, start_lock_mic_vol.bat** to:

     ```
     C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp
     ```
   * Disable `lock_mic_vol.bat` in autostart

     This will make it run every time Windows starts.
    * and now restart windows

## Use Pyvol_calc to calculate the volume
https://github.com/moxi-git/Lock-mic-vol/releases/download/idk/pyvol_calc.exe

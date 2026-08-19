# Circuit-SDK
# circuit_root

a lightweight, dark-themed administrative dashboard tool interface built for managing and optimizing la root environment states on the meta quest 3 standalone system platform using adb

---

##  important system warning
> **root can get ur headset bricked!!!! take this as a warning**  
> if you end up using perma root, meta may detect suspicious use, and ban u!!11!

---

## features

TypeScript injector
uhhhh
more
stuff
and more coming soon

---

## installation & compilation

### 1. environment preparation
ensure u have the necessary tools :
```bash
pip install windnd customtkinter pyinstaller
```

### 2. standalone binary building
to compress the tool layout script into a single, console-less windows desktop binary, execute the compilation string:
```bash
python -m pyinstaller --clean --onefile --noconsole --name="circuit_root" larp.py
```

### 3. file directory configuration
once compilation drops your finished executable inside the local `dist/` workspace folder, you **must** drop platform-tools-latest directly into that exact same directory location with it:
* `circuit_root.exe`
* `adb.exe`
* `adbwinapi.dll`
* `adbwinusbapi.dll`

---

## frida injections deployment steps

to utilize the interactive memory injection features successfully on an already-rooted device, you must hook up an interior listener daemon first:

1. download the matching official `frida-server` binary module framework built for **android-arm64**.
2. push the asset down into the headset temporary data storage layer:
   ```bash
   adb push frida-server /data/local/tmp/
   ```
3. escalate terminal execution permissions and trigger the server daemon persistently inside the background:
   ```bash
   adb shell "su -c 'chmod 755 /data/local/tmp/frida-server && /data/local/tmp/frida-server &'"
   ```
4. confirm that your target application package is actively open inside your headset lenses before firing the script compiler button in the ui dashboard layout.

---

## large syntax copy script

```batch
@echo off
echo --------------------------------------------------
echo   install required stuffaroo
echo --------------------------------------------------
echo.

echo installing customtkinter
python -m pip install windnd customtkinter pyinstaller

echo.
echo Larp
if not exist larp.py (
    echo [-] error: larp.py script missing from this directory folder path.
    pause
    exit
)

echo.
echo clean stuff
python -m pyinstaller --clean --onefile --noconsole --name="circuit_root" larp.py

echo.
echo ==================================================
echo   build process completed successfully!
echo   navigate into 'dist' and find da exe
echo ==================================================
pause
```


[yes i used ai for the README.md stop]

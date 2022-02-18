# Windows-Shortcuts


### Enable show more options by default while right clicking
Open cmd as administrator <br>
To enable this hack, paste the following and restart your computer
```
reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve
```
To disable this hack, paste the following and restart your computer
```
reg.exe delete "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}" /f
```


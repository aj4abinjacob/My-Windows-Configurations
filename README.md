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


### Make shortcuts for running python scripts
Run powershell as administrator <br>
paste the following
```
New-Item -Type file -Path $Profile -Force
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
notepad $Profile
```


A notepad will open, paste the commands below after replacing the file location with wherever you have saved the scripts and save it.
The function format is

function python_file_name{ python "file location" }

For example
	function combiner { python "C:\Users\abnjc\WorkScripts\FileCombiner.py" }   
	function splitfile { python "C:\Users\abnjc\WorkScripts\Splitfiletest.py" } 

Note:- The Shortcut shouldn’t have space between the words
Valid : function file_combiner { python "C:\Users\abnjc\WorkScripts\FileCombiner.py" }   
Not Valid : function file combiner { python “C:\Users\abnjc\WorkScripts\FileCombiner.py"}

## Windows Productivity tools
1. [Windows PowerToys](https://apps.microsoft.com/store/detail/microsoft-powertoys/XP89DCGQ3K6VLD)





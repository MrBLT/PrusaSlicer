# PrusaSlicer Instructions to Synchronize Settings
Git for windows is a prerequisite to running this script
1. Create a bat file in your download folder update_prusaslicer_config.bat
2. Set its contents to the following code
3. Run it
```bat
set repoauthor=MrBLT
set reponame=PrusaSlicer
set remotesource= https://github.com/%repoauthor%/%reponame%.git 

git clone %remotesource%

set source=%CD%/%reponame%
set destination=%appdata%\PrusaSlicer
robocopy %source% %destination% /mir /move
```

# PrusaSlicer

(update_prusaslicer_config.bat)
```bat
set repoauthor=MrBLT
set reponame=PrusaSlicer
set remotesource= https://github.com/%repoauthor%/%reponame%.git 

git clone %remotesource%

set source=%CD%/%reponame%
set destination=%appdata%\PrusaSlicer
robocopy %source% %destination% /mir /move
```
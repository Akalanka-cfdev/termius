@echo off

set BACKUP=D:\TermiusBackup

mkdir %BACKUP%

xcopy "%AppData%\Termius" "%BACKUP%\Termius" /E /I /Y
xcopy "%UserProfile%\.ssh" "%BACKUP%\.ssh" /E /I /Y

echo Backup Completed
pause

@echo off
color 4
:menu
cls
echo.
echo ===============================
echo     Please select an option:
echo ===============================
echo.
echo     1. IDM Activator
echo     2. Windows Activator
echo     3. Explorer Patcher
echo     4. Exit
echo.
echo ===============================
echo.
set /p option=[Enter your choice]:
if "%option%"=="1" goto IDM
if "%option%"=="2" goto Windows
if "%option%"=="3" goto Explorer
if "%option%"=="4" goto end
goto menu


:IDM
cls
echo Running IDM Activator...
powershell -Command "irm https://massgrave.dev/ias | iex"
pause
goto menu

:Windows
cls
echo Running Windows Activator...
powershell -Command "slmgr /skms kms8.msguides.com"
powershell -Command "slmgr /ato"
pause
goto menu

:Explorer
cls
echo Downloading Explorer Patcher...
powershell -Command "Invoke-WebRequest -Uri 'https://github.com/valinet/ExplorerPatcher/releases/latest/download/ep_setup.exe' -OutFile 'ep_setup.exe'"
explorer /select,%cd%\ep_setup.exe
pause
goto menu

:end
exit

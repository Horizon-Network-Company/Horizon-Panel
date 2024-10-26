# ✨Horizon Panel
<hr>

<img src="panel\public\img\Banner.png" style="border-radius: 21px">

<br/>

## Iniciar (Windows/Linux)
**txAdmin is included in all FXServer builds** above 2524, so to run it for the first time simply do the following:
- Update FXServer to the latest artifact/build (2524 or superior)
- If Windows, run FXServer.exe | If Linux, run `screen ./run.sh`
- Open one of the URLs shown and configure txAdmin

txAdmin requires to be launched from *inside* FXServer in monitor mode, to do that, just execute the `run.sh` or `FXServer.exe` without **any** `+exec` arguments.  
  
### ConVars
- **serverProfile:** The name of the server profile to start. Profiles are saved/loaded from the current directory inside the `txData` folder. The default is `default`.
- **txAdminPort:** The TCP port to use as HTTP Server. The default is `40120`.
- **txAdminInterface:** The interface to use as HTTP Server. The default is `0.0.0.0`.
- **txDataPath:** The path of the data folder. The default on Windows is `<citizen_root>/../txData` and on Linux `<citizen_root>/../../../txData`.
- **txAdminVerbose:** Set to `true` to print on the console more detailed information about errors and events. The default is `false`.
  
ConVar usage **example** for different port and profile:  
```bash
# Windows
./FXServer.exe +set serverProfile dev_server +set txAdminPort 40121

# Linux
./run.sh +set serverProfile dev_server +set txAdminPort 40121
```

### Contribucion y Desarollo
- All PRs should be based on the develop branch, including translation PRs.
- Before putting effort for any significant PR, make sure to join our discord and talk to us, since the change you want to do might not have been done for a reason or there might be some required context.
- If you want to run it from build & source, please do read [this](docs/development.md).


## Licencias, creditos y Agradecimientos
- This project is licensed under the [MIT License](https://github.com/tabarra/txAdmin/blob/master/LICENSE);
- ["Kick" button icons](https://www.flaticon.com/free-icon/users-avatar_8188385) made by __SeyfDesigner__ from [www.flaticon.com](https://www.flaticon.com);
- Warning Sounds ([1](https://freesound.org/people/Ultranova105/sounds/136756/)/[2](https://freesound.org/people/Ultranova105/sounds/136754/)) made by __Ultranova105__ are licensed under [CC 3.0 BY](http://creativecommons.org/licenses/by/3.0/);
- [Announcement Sound](https://freesound.org/people/IENBA/sounds/545495/) made by __IENBA__ is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/);
- [Message Sound](https://freesound.org/people/Divinux/sounds/198414/) made by __Divinux__ is licensed under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/);
- Especial thanks to everyone that contributed to this project, especially the very fine Discord folks that provide support for others;

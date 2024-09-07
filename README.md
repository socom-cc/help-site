## Community
- [Join the SOCOMPSP Discord](https://discord.gg/XtVYDr7) (official socom.cc Discord)
- [Join the PPSSPP Discord](https://discord.gg/5NJB6dD)

## Online games
- [Adhoc server games status](https://www.socom.cc/)
- [Active games in SOCOM FTB 2 infrastructure](https://psrewired.com/servers/20304) (*PS Rewired*)
- [Active games in SOCOM FTB 1 infrastructure](https://psrewired.com/servers/20034) (*PS Rewired*)
- [Other active infrastructure games PSP/PS2/PS3](https://psrewired.com/) (*PS Rewired*)

## Latest PPSSPP infrastructure build
Get the latest PPSSPP build with support for the infrastructure mode:
- [PPSSPP infra v1.16 Windows x64 with infra plugin](https://static.socom.cc/ppsspp/infra_windows/PPSSPP_1.16.6-806_win_x64_with_infra_plugin.zip)
- [PPSSPP infra v1.16 Windows ARM64 with infra plugin](https://static.socom.cc/ppsspp/infra_windows/PPSSPP_1.16.6-806_win_arm64_with_infra_plugin.zip)
- [PPSSPP infra v1.16 MacOS (SDL)](https://static.socom.cc/ppsspp/infra_mac/PPSSPP_1.16.6-806-g787afaa7c_infra_mac.zip)
- [PPSSPP infra v1.16 Linux (SDL)](https://static.socom.cc/ppsspp/infra_linux/PPSSPP_1.16.6-806-787afaa_infra_linux_SDL.zip)
- [PPSSPP infra v1.16 Android](https://static.socom.cc/ppsspp/infra_android/PPSSPP_1.16.6_infra_android.apk) ([recommended default ppsspp.ini file](https://static.socom.cc/ppsspp/infra_android/ppsspp.ini))
- [PPSSPP infra v1.16 iOS](https://static.socom.cc/ppsspp/infra_ios/PPSSPP_1.16.6-606_infra_iOS.ipa) ([recommended default ppsspp.ini file](https://static.socom.cc/ppsspp/infra_ios/ppsspp.ini))
- [See all the available builds here](https://static.socom.cc/ppsspp/)

Note the Windows infrastructure build is known for having issues with some revived infrastructure games.  
In that case, you might wanna use the Linux infrastructure build under [WSL](https://learn.microsoft.com/en-us/windows/wsl/about).  
For SOCOM: FTB 1, you may also need the [infra plugin v1.0.7](https://static.socom.cc/plugins/infra_plugin_107.zip).

## Recommended PPSSPP settings

### Graphics
- Backend: `Vulkan`
- Rendering resolution: `1:1`
- Hardware transform: `ON`
- Hardware tessellation: `ON`
- Anisotropic filtering: `16x`

### Networking
- Enable networking/WLAN: `ON`
- Change MAC address: If first time run, click `RANDOMIZE`
- WLAN channel: `Auto`
- Send Discord "Rich Presence" information: `ON`
- Enable built-in PRO ad hoc server: `OFF` (always, unless you host your own server with a PPSSPP instance)
- Enable UPnP: `ON` (automatically opens the appropriate ports, MUST ALSO be enabled in your modem/router settings)
- Port offset: `10 000`

### System
- Fast memory: `OFF`
- Cache full ISO in RAM: `ON`
- Change nickname: set it to your nickname (as seen on the [adhoc server games status](https://www.socom.cc/))

### Other settings
Open the `ppsspp.ini` configuration file in a text editor (close PPSSPP first if it's running).  
The file is located in PPSSPP's `memstick` folder, then in `PSP/SYSTEM/`.  
Find/add the following entries:

#### `General` section
- `EnablePlugins = True`
  
#### `Network` section
- `PrimaryDNSServer = 67.222.156.250`

You can then save the file, and run PPSSPP.

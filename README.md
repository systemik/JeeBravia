# JeeBravia
Jeedom Bravia Android TV 

Based on https://github.com/bunk3r/braviapy

Usage :

```
HELP :

$ ./jeebravia.py -h
Usage: jeebravia.py (-h|--help) (-p|--pin <pin>) (-v|--verbose) (-d|--discover) (-w|--wol <macaddr>) (-r|--remote) (-c|--command <command>)
    
DISCOVER :
$ ./jeebravia.py -d
Bravia found on 192.168.1.72

REMOTE CONTROL VIA SHELL :

$ ./bravia.py -r
[*] AccessControl
Registered!
CLIENTID=TVSideView:eb1214c4-321d-47ab-948d-9b9ebb36354e
NICKNAME=Jeedom (TV SideView)
[*] getRemoteControllerInfo
[p] PowerOff: AAAAAQAAAAEAAAAvAw==
[V] VolumeUp: AAAAAQAAAAEAAAASAw==
[v] VolumeDown AAAAAQAAAAEAAAATAw==
[C] ChannelUp AAAAAQAAAAEAAAAQAw==
[c] ChannelDown AAAAAQAAAAEAAAARAw==
[0] Num0: AAAAAQAAAAEAAAAJAw==
[1] Num1: AAAAAQAAAAEAAAAAAw==
[2] Num2: AAAAAQAAAAEAAAABAw==
[3] Num3: AAAAAQAAAAEAAAACAw==
[4] Num4: AAAAAQAAAAEAAAADAw==
[5] Num5: AAAAAQAAAAEAAAAEAw==
[6] Num6: AAAAAQAAAAEAAAAFAw==
[7] Num7: AAAAAQAAAAEAAAAGAw==
[8] Num8: AAAAAQAAAAEAAAAHAw==
[9] Num9: AAAAAQAAAAEAAAAIAw==
v
V
x
Remote Controller: exit!

VERBOSE MODE

$ ./bravia.py -v
[*] AccessControl
Registered!
CLIENTID=TVSideView:eb1214c4-321d-47ab-948d-9b9ebb36354e
NICKNAME=Jeedom (TV SideView)
Cookie: auth=ed06888a8b4f56bc47d61aaac6c8e93b044c936a87bd7342b10ff303717b2ebf; path=/sony/; max-age=1209600; expires=Wed, 05-Aug-2015 13:46:36 GMT;
[*] getPlayingContent
Program Title: In diretta dalla Camera dei Deputati "Question Time" Interrogazioni a risposta i
Title: Rai 2
MediaType: tv
RESULT:  [{"programTitle": "In diretta dalla Camera dei Deputati \"Question Time\" Interrogazioni a risposta i", "tripletStr": "318.1.3402", "title": "Rai 2", "durationSec": 4455, "uri": "tv:dvbt?trip=318.1.3402&srvName=Rai%202", "source": "tv:dvbt", "dispNum": "002", "startDateTime": "2015-07-22T15:00:00+0200", "programMediaType": "tv"}]

[*] getSystemInformation
[
    {
        "product": "TV",
        "macAddr": "B0:10:41:72:C6:83",
        "name": "BRAVIA",
        "language": "ita",
        "cid": "1F74D30894F5121275F41A2B8EB9337DD62C1543",
        "generation": "2.4.1",
        "region": "ITA",
        "area": "ITA",
        "model": "KDL-50W705B",
        "serial": "01010101"
    }
]


SEND COMMAND

$ ./jeebravia.py -c Volume Up

LIST OF KNOWN COMMANDS:

Num1
Num2
Num3
Num4
Num5
Num6
Num7
Num8
Num9
Num0
Num11
Num12
Enter
GGuide
ChannelUp
ChannelDown
VolumeUp
VolumeDown
Mute
TvPower
Audio
MediaAudioTrack
Tv
Input
TvInput
TvAntennaCable
WakeUp
PowerOff
Sleep
Right
Left
SleepTimer
Analog2
TvAnalog
Display
Jump
PicOff
PictureOff
Teletext
Video1
Video2
AnalogRgb1
Home
Exit
PictureMode
Confirm
Up
Down
ClosedCaption
Component1
Component2
Wide
EPG
PAP
TenKey
BSCS
Ddata
Stop
Pause
Play
Rewind
Forward
DOT
Rec
Return
Blue
Red
Green
Yellow
SubTitle
CS
BS
Digital
Options
Media
Prev
Next
DpadCenter
CursorUp
CursorDown
CursorLeft
CursorRight
ShopRemoteControlForcedDynamic
FlashPlus
FlashMinus
AudioQualityMode
DemoMode
Analog
Mode3D
DigitalToggle
DemoSurround
*AD
AudioMixUp
AudioMixDown
PhotoFrame
Tv_Radio
SyncMenu
Hdmi1
Hdmi2
Hdmi3
Hdmi4
TopMenu
PopUpMenu
OneTouchTimeRec
OneTouchView
DUX
FootballMode
iManual
Netflix
Assists
FeaturedApp
FeaturedAppVOD
GooglePlay
ActionMenu
Help
TvSatellite
WirelessSubwoofer
```

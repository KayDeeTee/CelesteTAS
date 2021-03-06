# CelesteTAS
Simple TAS Tools for the game Celeste

## Installation
- Go to [Releases](https://github.com/ShootMe/CelesteTAS/releases)
- Download Celeste-Addons.dll
- You will need the modified Celeste.exe as well. I wont host it here.
  - You can modify it yourself with dnSpy or similar
  - Load Celeste.exe in dnSpy and Celeste-Addons.dll as well
  - Change Celeste.exe according to the document here [Modified](https://github.com/ShootMe/CelesteTAS/blob/master/Game/WhatsModified.txt)
  - Save the modified version and you should be good to go
- Place those in your Celeste game directory (usually C:\Program Files (x86)\Steam\steamapps\common\Celeste\)
- Make sure to back up the original Celeste.exe before copying. (Can rename them .bak or something)
- For playback to be correct, make sure Jump is bound to 'A', Dash is bound to 'B', Grab is bound to 'RB', Quick Reset is bound to 'LB', and talk is bound to 'B'

## Input File
Input file is called Celeste.tas and needs to be in the main Celeste directory (usually C:\Program Files (x86)\Steam\steamapps\common\Celeste\Celeste.tas)

Format for the input file is (Frames),(Actions)

ie) 123,R,J (For 123 frames, hold Right and Jump)

## Actions Available
- R = Right
- L = Left
- U = Up
- D = Down
- J = Jump
- X = Dash
- G = Grab
- S = Start
- Q = Quick Reset

## Special Input
- You can create a break point in the input file by typing *** by itself on a single line
- The program when played back form the start will go very fast till it reaches that line and then go into frame stepping mode

## Playback / Recording of Input File
### Controller
While in game
- Playback: Left Trigger + Right Trigger + Right Stick
- Stop: Left Trigger + Right Trigger + DPad Down
- Record: Left Trigger + RIght Trigger + Left Stick
- Faster Playback: Right Stick X+
- Frame Step: DPad Up
- While Frame Stepping:
  - One more frame: DPad Up
  - Continue at normal speed: DPad Down
  - Frame step continuously: Right Stick X+

### Keyboard
While in game
- Playback: Control + [
- Stop: Control + ]
- Record: Control + Backspace
- Faster/Slower Playback: RightShift / LeftShift
- Frame Step: [
- While Frame Stepping:
  - One more frame: [
  - Continue at normal speed: ]
  - Frame step continuously: RightShift
  
## Celeste Studio
Can be used instead of notepad or similar for easier editing of the TAS file. Is located in [Releases](https://github.com/ShootMe/CelesteTAS/releases) as well.

If Celeste.exe is running it will automatically open Celeste.tas if it exists. You can hit Ctrl+O to open a different file, which will automatically save it to Celeste.tas as well. Ctrl+Shift+S will open a Save As dialog as well.

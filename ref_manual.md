# STELLA Reference Manual 
---
###### ^
## Contents
- [Interface Commands]
  - [Add Cursor Preset]
  - [Add Cursor to Preset]
  - [Activate Voice]
  - [Capture Audio]
  - [Capture Video]
  - [Change Cursor]
  - [Change Settings]
  - [Change Screen]
  - [Close]
  - [Close Console]
  - [Close Log Editor]
  - [Define]
  - [Display Screen Information]
  - [Download Expr]
  - [Elevate Perms]
  - [Flush Logs]
  - [Force Logging Flush]
  - [Hide Console]
  - [Load Cursor Preset]
  - [Move]
  - [Open Console]
  - [Open Log Editor]
  - [Open Logs]
  - [Play Audio]
  - [Plot]
  - [Print Element Details]
  - [Random Cat Picture]
  - [Record Audio]
  - [Record Screen]
  - [Remove Cursor from Preset]
  - [Reset Cursor]
  - [Save Plot]
  - [Screenshot]
  - [See Settings]
  - [Set]
  - [Show Console]
  - [Show Live Logger]
  - [Show Logger]
  - [Show Screen Info]
  - [Start Audio Capture]
  - [Start Monitoring Process]
  - [Start Process Measuring]
  - [Start Recording]
  - [Stop Audio]
  - [Stop Audio Capture]
  - [Stop Audio Recording]
  - [Stop Monitoring Process]
  - [Stop Process Measuring]
  - [Stop Recording]
  - [Stop Video]
  - [Take Process Snapshot]
  - [Test Error]
  - [Toggle Cursor Effects]
  - [View Log]
  - [View Settings]
  - [Write R6 Scores]
  - [Write Schema]
- [Shortcuts]
	- oii
- [Menus]
	- oii
---
## Interface Commands
### Add Cursor Preset
- Aliases: acp, create cursor preset
- Command Index: 31
- Description: Creates a new cursor preset
- Associated Shortcut: No Shortcut.
- Parameters: listname{string}

^[^]^
### Add Cursor to Preset
- Aliases: actp
- Command Index: 32
- Description: Adds a cursor to a preset
- Associated Shortcut: No Shortcut.
- Parameters: preset{string}, cursorid{string}, filepath{string}

^[^]^
### Activate Voice
- Aliases: No Aliases.
- Command Index: 38
- Description: Activates voice recognition
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Capture Audio
- Aliases: ca, begin audio capture, start audio capture, record audio, start recording audio
- Command Index: 5
- Description: Starts capturing system audio, with optional audio input (0/exclusive, 1/inclusive).
  E.g: capture audio ;exclusive
  E.g: capture audio ;1
- Associated Shortcut: No Shortcut.
- Parameters: [mode{int/string}]

^[^]^
### Capture Video
- Aliases: cv, begin video capture, start video capture, record screen, start recording
- Command Index: 4
- Description: Begins capturing screen as a video, mutlimonitor support coming soon. Closes the interface when ran.
- Associated Shortcut: Shifts Q R
- Parameters: No Parameters.

^[^]^
### Change Cursor
- Aliases: cc, change mouse
- Command Index: 15
- Description: (Attempts to) Changes the cursor to the specified cursor file, specifying file path.
  E.g: change cursor ;the/path/to/your/.cur/file
- Associated Shortcut: No Shortcut.
- Parameters: path{string}

^[^]^
### Change Settings
- Aliases: cs, edit settings, set
- Command Index: 9
- Description: Changes a control setting, you must specify the 
  E.g: change setting ;LogAssemblies ;true
  E.g: change setting ;background ;green
- Associated Shortcut: No Shortcut.
- Parameters: variablename{string}, value{string}

^[^]^
### Change Screen
- Aliases: move, relocate
- Command Index: 2
- Description: Shifts the interface screen to another monitor, takes in a number corresponding to the monitor you want it to shift to (1 being primary)
- Associated Shortcut: Shifts Q (number)
- Parameters: screennum{int}

^[^]^
### Close
- Aliases: hide, cls
- Command Index: 1
- Description: Closes the interface, the shortcut will open it.
- Associated Shortcut: Shifts Q I
- Parameters: No Parameters.

^[^]^
### Close Console
- Aliases: hll, close live logger, hide live logger, close logger, hide logger
- Command Index: 23
- Description: Closes an open live logger
  E.g: cll
- Associated Shortcut: Shifts Q .
- Parameters: No Parameters.

^[^]^
### Close Log Editor
- Aliases: cle
- Command Index: 39
- Description: Closes the log editor
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Define
- Aliases: No Aliases.
- Command Index: 40
- Description: Defines a word using the DictionaryAPI or the UrbanDictionaryAPI (if allowed)
- Associated Shortcut: No Shortcut.
- Parameters: word{string}

^[^]^
### Display Screen Information
- Aliases: dsi, show screen info, ssi, show screen information
- Command Index: 21
- Description: Displays either all screen information, or just a specified one.
  dsi ;1
- Associated Shortcut: No Shortcut.
- Parameters: [screennumber{int}]

^[^]^
### Download Expr
- Aliases: No Aliases.
- Command Index: 27
- Description: Downloads exprs
- Associated Shortcut: No Shortcut.
- Parameters: processname{string}

^[^]^
### Elevate Perms
- Aliases: ep
- Command Index: 36
- Description: Restarts the application asking for elevation (admin)
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Flush Logs
- Aliases: flf, force log flush, force flush logs
- Command Index: 26
- Description: Forces a logging flush
- Associated Shortcut: Shifts Q F
- Parameters: No Parameters.

^[^]^
### Force Logging Flush
- Aliases: No Aliases.
- Command Index: 26
- Description: Forces a logging flush
- Associated Shortcut: Shifts Q F
- Parameters: No Parameters.

^[^]^
### Hide Console
- Aliases: close console, close live logger, hide live logger, close logger, hide logger
- Command Index: 23
- Description: Closes an open live logger
  E.g: cll
- Associated Shortcut: Shifts Q .
- Parameters: No Parameters.

^[^]^
### Load Cursor Preset
- Aliases: lcp, load cursors
- Command Index: 30
- Description: Loads a specified cursor preset
- Associated Shortcut: No Shortcut.
- Parameters: listname{string}, [persistent{bool}]

^[^]^
### Move
- Aliases: change screen, relocate
- Command Index: 2
- Description: Shifts the interface screen to another monitor, takes in a number corresponding to the monitor you want it to shift to (1 being primary)
- Associated Shortcut: Shifts Q (number)
- Parameters: screennum{int}

^[^]^
### Open Console
- Aliases: sll, show live logger, open live logger, show logger, open logger
- Command Index: 22
- Description: Opens the live logger.
  E.g:sll
- Associated Shortcut: Shifts Q ,
- Parameters: No Parameters.

^[^]^
### Open Log Editor
- Aliases: ole
- Command Index: 35
- Description: Opens the log editing GUI
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Open Logs
- Aliases: open log folder, ol, olf
- Command Index: 13
- Description: Opens the logs folder.
  E.g: open logs
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Play Audio
- Aliases: start playing audio, run audio file, play audio file, pa
- Command Index: 8
- Description: Plays an audio file, present the filepath as an argument with optional looping.
  E.g: play audio ;C:/Downloads/Sussyaudio.mp4 ;true
- Associated Shortcut: No Shortcut.
- Parameters: filepath{str}, [looping{bool}]

^[^]^
### Plot
- Aliases: plot data, plot graph, create graph, pd
- Command Index: 17
- Description: Plots a set of data, specifying file path(s) or data in the format: ;int, int, int, ... int ;int, int, int, ... int (two sets of data).
  E.g: plot ;path/to/a/csv/with/two/lines/of/data
  E.g: plot ;path/to/csv/with/x_axis/data ;path/to/2nd/csv/with/y_axis/data
  E.g: plot ;1, 2, 3, 4, 5, 6 ;66, 33, 231, 53242, 564345
- Associated Shortcut: No Shortcut.
- Parameters: filepath{string} | filepath1{string} filepath2{string} | data1{int[]} data2{int[]}

^[^]^
### Print Element Details
- Aliases: ped
- Command Index: 25
- Description: Prints the interface element details
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Random Cat Picture
- Aliases: cat, rcp, random cat, cat picture, kitty, kitty cat
- Command Index: 19
- Description: Shows a random kitty :3
- Associated Shortcut: Shifts Q K
- Parameters: No Parameters.

^[^]^
### Record Audio
- Aliases: ca, begin audio capture, start audio capture, start recording audio
- Command Index: 5
- Description: Starts capturing system audio, with optional audio input (0/exclusive, 1/inclusive).
  E.g: capture audio ;exclusive
  E.g: capture audio ;1
- Associated Shortcut: No Shortcut.
- Parameters: [mode{int/string}]

^[^]^
### Record Screen
- Aliases: cv, capture video, begin video capture, start video capture, start recording
- Command Index: 4
- Description: Begins capturing screen as a video, mutlimonitor support coming soon. Closes the interface when ran.
- Associated Shortcut: Shifts Q R
- Parameters: No Parameters.

^[^]^
### Remove Cursor from Preset
- Aliases: rcfp
- Command Index: 33
- Description: Removes a cursor from a preset
- Associated Shortcut: No Shortcut.
- Parameters: preset{string}, cursorid{string}

^[^]^
### Reset Cursor
- Aliases: rc, reset mouse
- Command Index: 16
- Description: Resets all system cursors
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Save Plot
- Aliases: sp, save plotted data, save plot data, save graph
- Command Index: 18
- Description: Saves a currently open plot (Plot must be open) to a file.
  E.g: save plot
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Screenshot
- Aliases: ss, take screenshot, screen capture
- Command Index: 3
- Description: Takes a screenshot of the screen, without the interface. -2 for a stiched image of all screens, -1 for individual screen pics, (number) for an individual screen, leave empty for the current screen Kitty is running on.
  E.g: screenshot ;-2
- Associated Shortcut: Shifts Q S
- Parameters: [mode{int}]

^[^]^
### See Settings
- Aliases: view settings, print settings, vs
- Command Index: 29
- Description: Prints all user settings in the format:
  [Section]
    [Key]: [Value]
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Set
- Aliases: cs, edit settings, change setting
- Command Index: 9
- Description: Changes a control setting, you must specify the 
  E.g: change setting ;LogAssemblies ;true
  E.g: change setting ;background ;green
- Associated Shortcut: No Shortcut.
- Parameters: variablename{string}, value{string}

^[^]^
### Show Console
- Aliases: sll, open console, show live logger, open live logger, show logger, open logger
- Command Index: 22
- Description: Opens the live logger.
  E.g:sll
- Associated Shortcut: Shifts Q ,
- Parameters: No Parameters.

^[^]^
### Show Live Logger
- Aliases: sll, open console, open live logger, show logger, open logger
- Command Index: 22
- Description: Opens the live logger.
  E.g:sll
- Associated Shortcut: Shifts Q ,
- Parameters: No Parameters.

^[^]^
### Show Logger
- Aliases: sll, open console, show live logger, open live logger
- Command Index: 22
- Description: Opens the live logger.
  E.g:sll
- Associated Shortcut: Shifts Q ,
- Parameters: No Parameters.

^[^]^
### Show Screen Info
- Aliases: dsi, display screen information, ssi, show screen information
- Command Index: 21
- Description: Displays either all screen information, or just a specified one.
  dsi ;1
- Associated Shortcut: No Shortcut.
- Parameters: [screennumber{int}]

^[^]^
### Start Audio Capture
- Aliases: ca, begin audio capture, record audio, start recording audio
- Command Index: 5
- Description: Starts capturing system audio, with optional audio input (0/exclusive, 1/inclusive).
  E.g: capture audio ;exclusive
  E.g: capture audio ;1
- Associated Shortcut: No Shortcut.
- Parameters: [mode{int/string}]

^[^]^
### Start Monitoring Process
- Aliases: spm, monitor process, smp, mp
- Command Index: 11
- Description: Starts measuring a processes's information until stopped.
  E.g: start measuring process ;devenv
- Associated Shortcut: Shifts Q X
- Parameters: No Parameters.

^[^]^
### Start Process Measuring
- Aliases: spm, monitor process, smp, mp
- Command Index: 11
- Description: Starts measuring a processes's information until stopped.
  E.g: start measuring process ;devenv
- Associated Shortcut: Shifts Q X
- Parameters: No Parameters.

^[^]^
### Start Recording
- Aliases: cv, capture video, begin video capture, start video capture, record screen
- Command Index: 4
- Description: Begins capturing screen as a video, mutlimonitor support coming soon. Closes the interface when ran.
- Associated Shortcut: Shifts Q R
- Parameters: No Parameters.

^[^]^
### Stop Audio
- Aliases: sap, stop audio playback, abort audio playback, abort audio
- Command Index: 24
- Description: Aborts a currently playing audio file.
- Associated Shortcut: Shifts Q V
- Parameters: No Parameters.

^[^]^
### Stop Audio Capture
- Aliases: sar, stop audio recording, stop recording audio
- Command Index: 7
- Description: Stops a currently running audio session, with optional opening of the file location after saving.
  E.g: stop audio ;true
- Associated Shortcut: No Shortcut.
- Parameters: 

^[^]^
### Stop Audio Recording
- Aliases: sar, stop recording audio, stop audio capture
- Command Index: 7
- Description: Stops a currently running audio session, with optional opening of the file location after saving.
  E.g: stop audio ;true
- Associated Shortcut: No Shortcut.
- Parameters: 

^[^]^
### Stop Monitoring Process
- Aliases: stop measuring process, finish process measuring, finish measuring process, finish process measurements, finish process recording, fpm, finish process monitor, finish monitoring process, fmp
- Command Index: 12
- Description: Stops a currently running process measuring session, with an optional saving of the data.
  E.g: stop measuring process ;false
- Associated Shortcut: Shifts Q C
- Parameters: [savedata{bool}]

^[^]^
### Stop Process Measuring
- Aliases: finish process measurements, finish process recording, fpm, finish process monitor, finish monitoring process, fmp
- Command Index: 12
- Description: Stops a currently running process measuring session, with an optional saving of the data.
  E.g: stop measuring process ;false
- Associated Shortcut: Shifts Q C
- Parameters: [savedata{bool}]

^[^]^
### Stop Recording
- Aliases: stop video, sv, stop video recording, stop recording video, stop video capture, stop screen capture, stop screen recording
- Command Index: 6
- Description: Stops a currently running recording session, with an optional opening of the recording location after saving (true)
  E.g: stop recording ;true
- Associated Shortcut: Shifts Q D
- Parameters: No Parameters.

^[^]^
### Stop Video
- Aliases: sv, stop video recording, stop recording video, stop video capture, stop screen capture, stop screen recording
- Command Index: 6
- Description: Stops a currently running recording session, with an optional opening of the recording location after saving (true)
  E.g: stop recording ;true
- Associated Shortcut: Shifts Q D
- Parameters: No Parameters.

^[^]^
### Take Process Snapshot
- Aliases: tps
- Command Index: 10
- Description: Takes a 'snapshot' of a specified process and shows information like it's memory usage, cpu usage, etc.
  E.g: take process snapshot ;devenv
  E.g: take process snapshot ;9926381232
- Associated Shortcut: Shifts Q T
- Parameters: process{string/int}

^[^]^
### Test Error
- Aliases: No Aliases.
- Command Index: 37
- Description: [DEBUG] Throws an error
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Toggle Cursor Effects
- Aliases: tce
- Command Index: 46
- Description: Toggles Cursor effects!
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### View Log
- Aliases: open log, vl
- Command Index: 14
- Description: Opens a specified log file for viewing, specifying index or name.
  E.g: view log ;1
  E.g: view log ;Lcc0648800552499facf099d368686f0c
- Associated Shortcut: No Shortcut.
- Parameters: filename{string/int}

^[^]^
### View Settings
- Aliases: see settings, print settings, vs
- Command Index: 29
- Description: Prints all user settings in the format:
  [Section]
    [Key]: [Value]
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Write R6 Scores
- Aliases: wr6s
- Command Index: 41
- Description: Writes the preset r6 data to stats.bin
- Associated Shortcut: No Shortcut.
- Parameters: No Parameters.

^[^]^
### Write Schema
- Aliases: No Aliases.
- Command Index: 44
- Description: Writes a sequence of types to a schema in the format 'schema_name name type {type name}' (one or more pairs of 'type name'). 
  E.g: 
     Character string name int kills int deaths
     ^ Name ^ Type ^ Name ^ Type ^ Name
  E.g: 
     Map string name double size_w double size_h List characternames
- Associated Shortcut: No Shortcut.
- Parameters: name{string}, types_list{string}

---

## Shortcuts

^[^]^
### Toggle Interface
- Shortcut: `LShift` `RShift` `Q` `I`
- Description: Toggles the interface

^[^]^
### Toggle Interface
- Shortcut: `Q` `I` `C`
- Description: Toggles the cursor effects

^[^]^
### Shutdown
- Shortcut: `LShift` `RShift` `Q` `E`
- Description: Shutsdown the program

^[^]^
### Load Cursor Preset
- Shortcut: `Q` `C` `1/2/3/4/5/6/7/8/9`
- Description: Toggles the interface

^[^]^
### Reset Cursor
- Shortcut: `Q` `C` `0`
- Description: Resets the cursor to the default
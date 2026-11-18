# Changelog

Every build of Stillward Display that goes out on Steam, newest first. Each
one is also a [release](https://github.com/ayokiru/stillward-display/releases)
here: choose Watch → Custom → Releases to hear about them.

Stillward Display is out on Steam:
[get it there](https://store.steampowered.com/app/5248400/Stillward_Display/).

## 2.0.1432

Uploaded to Steam on 18 November 2026, six days after 2.0.1395. It brings 37 changes: a new taskbar look, running programs you can put in your own order, an island note you can edit like any text field, and fixes for shutting down from Stillward's power menu and for live wallpapers under its taskbar.

### Taskbar and dock

- Running programs keep their places. They used to jump ahead every time you switched to one. Now they stay in the order they started, after the pinned ones: a program you start goes to the end, and one you close leaves. Drag a running program over another to swap them, on any bar or the dock.
- Stillward's taskbar can stand on every screen or on the main screen only, from the Screens row on the Taskbar page. The taskbar builder asks the same: every monitor alike, the main monitor only, or a different bar on the other monitors.
- The option that slides the dock and the island away now reads "While a window is maximized".
- A look made in the taskbar builder opens in the builder again, and Keep as a look saves over it.
- A new look on the Workshop, Steel dock, corners below: the power menu and your desktops in the bottom left corner, your programs on steel in the middle, growing under the pointer, the tray, language, network, volume and notifications in the bottom right, and the top of the screen left free for the island.
- Workshop pictures of taskbars that run the full width of the screen now show the whole bar. Three islands, Studio, Quiet row and Taskbar on top had a corner cut off.
- Stillward's taskbar and dock redraw only when something on them changes. A window changing its title or the pointer passing over used to be enough to redraw a strip as wide as the screen, which could make a live wallpaper under it stutter, most of all on a second monitor.
- If Explorer wasn't ready at sign-in, the dock tries again to hide the Windows taskbar, so the two no longer stay on the screen together.
- When the Windows key opens Apps while no Stillward taskbar or dock is on, the Now page says so.

### The island

- Calls is a switch of its own on the Island page, off by default. With it off, a program using the microphone or the camera no longer opens the island.
- Starting a timer opens the island for a moment, with the time in large figures and a ring filling around the timer icon. Then it folds back, and the ring runs down with the time left.
- The note has a caret. Click to place it, drag to select, double-click to select a word, and use the arrows, Home and End, with Shift to select and Ctrl to move by words. Typing, pasting, Backspace and Delete work at the caret or on the selection, and the four lines shown follow the caret through a longer note.
- The island's clock takes the typeface of the activity around it.
- Clicking the player on the island brings the player's window to the front.

### Screenshots

- Saved colours: the cross on a colour under the pointer, or a right-click, removes it, and you can drag colours into your own order.
- Click the colour's code under the wheel to type one in: #3f4447, #fa0, 63, 68, 71 or rgb(63, 68, 71).
- Snap to windows on the Capture page can be turned off, and holding Alt turns it off for the moment, so an area can start on top of a window.
- Esc removes a screenshot pinned over other windows (Ctrl+P) while the pointer is over it.

### New

- Restart in the tray menu, beside Quit. The program closes, puts everything back and comes up again in the tray, without going through Steam.
- Apps (the Win key) finds Stillward Display itself.
- The help page links the Discord server, under Send feedback.
- The Workshop cards of pointer sets show the pointers sharper.

### Fixes

- Restart and Shut down from Stillward's power menu could end in nothing. Putting things back first now takes 15 seconds at most, and if Windows refuses, a card says so with the error code.
- Restoring a window could flash the whole window before Stillward's animation began, when Windows' own animation had been switched back on behind its back. Stillward now keeps Windows' animation off for as long as one of its own is chosen.
- The volume keys follow the output you switched to, such as headphones, and no longer the one active when the program started.
- Widgets and the island's calendar buttons show their icons on Windows 10, where they were empty boxes.
- The control centre's tile rows on the Taskbar page no longer overlap in a narrow window.
- The widget editor's Fit enlarges very small cards enough to see them.

## 2.0.1395

Uploaded to Steam on 12 November 2026, six days after 2.0.1329. It brings 66 changes: colours of your own for marking up screenshots, clicks you can see in a recording, and a round of fixes from testers' reports.

### Screenshots and recordings

- The ring of tools around a screenshot now has an eyedropper and a palette. The eyedropper takes a colour from anything on the screen. The palette (C) opens a colour wheel: hue around it, saturation out from the middle, brightness on a bar underneath.
- Any colour, taken with the eyedropper or picked on the wheel, can be saved. Saved colours stay from one capture to the next. They show up in the side panel, in the right-click ring of colours and under the wheel, so the next screenshot starts with them. Up to twelve are kept, and saving a colour that is already saved removes it.
- Marks on a video are drawn in the same editor, so they get all of this too.
- Clicks in the video: a new button among the recording's buttons (C), and a switch on the Capture page, put a ring on every click while the recording runs. The rings switch off by themselves when the recording ends. They show in recordings of a screen or an area; a window recorded on its own is captured without them.
- The recording's buttons now stand above Stillward's own dock and taskbar instead of on them.

### Fixes

- Minimising the last window on a desktop animates again. Before, the window just vanished.
- A window joining a group of tabs no longer flashes a white plate, in browsers and chat programs too.
- Windows join as tabs only when you let go of one on a strip of tabs. Moving a window past another's title bar used to join them unasked, and a tab pulled off could snap back. The strip also stays open while the pointer travels up to it.
- The island's note now does select all, copy, cut and paste, whatever the keyboard layout.
- The island no longer shows a call for a program that isn't running. A program closed while using the microphone used to stay marked as using it.
- Files dropped on the island keep its shelf open for a moment, so you see them land.
- The dock's menus open from the dock, and the dock never sits under a Stillward taskbar.
- "Put it back" on the Taskbar page brings the Windows taskbar back, and switches off Stillward's dock and bar along with it.
- The taskbar builder puts a part where you drop it on a bar along the top of the screen.
- The Apps search field (the Win key) selects, copies and cuts with Ctrl+A, Ctrl+C and Ctrl+X.
- "As it was" after a setup brings back your own dock size, not the size from the look.
- A few lists could show internal names instead of words if they were opened before the language had loaded: the widget shelves, the icon sets, the control centre. They show the words now.

### For creators

- Island activities and setups open from a file, or dropped on the window, like the other formats. The [creators' files](https://github.com/ayokiru/stillward-display/tree/main/creators) already follow this.

## 2.0.1329

Uploaded to Steam on 6 November 2026. The previous public build was 0.9.350, uploaded on 9 October. The last number in the version counts the changes made to the program since its first line of code: 350 then, 1,329 now, so 979 of them landed in these four weeks. In that time the program went from arranging windows and screens for games to reshaping most of the Windows desktop, and the version went from 0.9 to 2.0.

All of it still works from outside other programs. Nothing is injected into games or apps, and everything the program changes in Windows goes back when you turn it off or uninstall it, and after a crash.

### Window animations

Windows animates a window the same way every time and offers no choice. Stillward Display 2.0 replaces these animations with its own, chosen separately for each moment:

- minimising and restoring
- maximising and going full screen
- dragging a window
- snapping it to a zone
- opening and closing (closing works from the X button too)
- switching between windows
- applying a layout
- moving a window to another monitor
- switching virtual desktops, where windows slide out and the new desk slides in

There are close to a hundred styles: springs, jelly, glass, a window that rolls up like a blind, one that pours into its taskbar button, one that burns away, and many more. Most come through Steam Workshop, so new ones arrive without an update. A built-in editor lets anyone make their own, down to a grid effect where every point of the window moves on its own timeline, and publish it. A window can also be thrown with the mouse, and "Show desktop" sends windows off to the screen edges and brings them back along the same path.

One slider sets the speed of all the program's animations.

### Your own taskbar and Start

The program can now hide the Windows taskbar completely and put its own in its place, on every monitor:

- a full taskbar or a dock, at any edge or floating, with magnification and live window previews
- built from "islands" of parts: apps, clock, tray, volume, music, control centre
- its own system tray, or none
- glass that stays readable on any wallpaper, with one slider from clear to tinted
- the Win key opens the program's own Apps view instead of Start: search across apps, files, folders and Windows settings, plus a power menu
- volume on the scroll wheel over the taskbar, and per app over its button
- the volume keys show the level on the program's own bar instead of Windows' box over the dock

Taskbar looks are shared through the Workshop. People who keep the Windows taskbar can still change its native settings per preset or per desk (position, size, alignment, grouping, seconds on the clock) and have it hide while a window is maximised.

### The island

A small dark pill at the top of every screen shows what's going on and opens when you point at it:

- music, tinted by the album cover, with playback controls
- a recording in progress, a timer, a "keep awake" timer
- camera or microphone in use
- what was just copied, and a shelf to drop files on
- battery, volume, the clock with a calendar
- streaming mode on or off

What the island shows is made of "activities", and new ones come from the Workshop, along with motion add-ons such as glow and jelly edges.

### Setups, and the Workshop for everything you see

The Workshop now carries every visual part of the desktop: animation styles, taskbar looks, pointer sets, widgets, island activities and icon sets. On top of them sits the Setup, one item that holds a whole desk: animations, taskbar, pointer, island, widgets, wallpaper, colours and icons.

- take a whole Setup or only the parts you want, and get your old desk back with one button
- share your own as a Setup, or send it to a friend as a link or a short code
- a preset or a time of day can put a Setup on and take it off again
- "Surprise me" builds a random desk from what you have, with locks on parts you want to keep
- authors can mark what subscribers may adjust, such as a colour, a speed or a size, within limits they set
- the Workshop opens inside the program with popular, new and this week's items, a Setup of the week and seasonal collections

Every Workshop item is pictured on the same sample desk, so a look in the list is the look you get.

### Screenshots

The program now takes screenshots itself:

- one key for a window (exactly its frame, no shadow), a zone, a monitor or every monitor at once
- an overlay with tools around the selection: crop, arrows, boxes, text, blur, fixed aspect ratios and exact pixel sizes
- HDR screenshots that look like the screen, not grey and washed out
- a clean frame: desktop icons, taskbar, notifications and the program's own layers hidden, chosen apps (chat, mail, passwords) blurred
- emails, IP addresses, keys and card numbers found and pixelated automatically
- copy the text from a screenshot, read a QR code, pick a colour, measure with a ruler
- a long screenshot of a scrolling window, captured without touching the mouse
- pin a screenshot on top of a game, see-through and click-through
- a styled shot of a window on a steel background with rounded corners and a soft shadow, ready to post
- files sorted into a folder per game, and a button that sends a shot to the Steam screenshot library

### Screen recording

- one key to start, pause and stop, on the graphics card's own encoder
- scenes: a window that the frame follows, a zone, a monitor, the whole desk, or a vertical 9:16 frame for shorts
- the whole desk in one video, even with mixed resolutions and refresh rates
- separate audio tracks for the system, the microphone and a single game or app
- keep the last 30 seconds to 5 minutes in memory and save them with a key
- the clean frame and blur work through the whole recording
- annotations on video, trimming, cutting, joining, speed changes and muting tracks, all on a copy
- export to fit a size limit (10, 25, 50 MB), as a GIF or as audio only
- studio recording: the program follows the clicks with a smooth zoom and smooths the pointer's path
- HDR recordings come out with normal colours
- one feed of recent screenshots and recordings in the window

### Windows that behave the way you want

Ideas people know from other desktop systems, brought to Windows without injection:

- window rules: an app always opens on its monitor, zone or virtual desktop
- tabs: drop one window on another's title bar and they become one window with tabs
- a scrolling strip: windows side by side in columns wider than the screen, scrolled with a key or the wheel
- maximise inside a zone instead of the whole screen, and automatic tiling
- window overview: every window on a monitor spread out as live pictures
- hot corners: point at a corner to run an action
- shelf: shake the pointer while dragging a file and a shelf appears to collect files on
- quick look: press Space on a file in Explorer to preview pictures, video, PDF, text and code
- control centre: tiles you arrange yourself across pages, for presets, sound, Wi-Fi, keep awake and more
- bedside clock mode: a big clock, widget stacks or a photo frame on a chosen monitor, dimmed red at night
- music shown as a live spectrum on the bar, dock, island or a widget
- a drop-down window from the screen edge for any app, on a key
- minimise any window to the tray, or roll it up to its title bar
- picture-in-picture: a live copy of any window, or part of one, on top of a game
- desktop shelves showing a folder's contents

And small keys: cycle the windows of the app in front, reopen the last window you closed, paste as plain text, jump the pointer to the next monitor, and stop the pointer getting stuck between monitors of different heights.

### Pointer

- replaces the system pointers with sets that are drawn at the exact size for each monitor's scale
- a pointer studio with a generator (sliders rebuild all 17 pointer shapes) and a vector editor
- animated pointers, and effects such as trails, sparks and click rings
- a key that shows where the pointer is
- its own pointer for a single app
- sets are shared through the Workshop

### Widgets

More than twenty widgets for the desktop: clocks, CPU, memory, graphics card and network load, what's playing, volume, the program's own desks and presets. A widget studio starts from a gallery or a blank skeleton, lets you change content, style and effects, and publishes to the Workshop.

### The look of the whole desktop

- each desk or preset has its own wallpaper per monitor, light or dark theme, accent colour and pointer
- the accent colour taken from the wallpaper, and recalculated when the wallpaper changes
- wallpapers by time of day and per virtual desktop
- window borders and title bars in the brand, accent or your own colour, rounded or square corners, or no coloured border at all
- dark title bars and the translucent Windows backdrop on other apps' windows
- a coloured frame or glow around the active window
- icon sets for the dock, taskbar, folders, desktop icons and file types
- folder colours, desktop icon size and arrangement, the Recycle Bin and This PC icons
- the lock screen follows the desk's look
- a screensaver and idle screen with a clock, the wallpaper or a slowly shifting dark screen for OLED
- Windows' own sounds replaced by the program's sound set, and optional sounds for window events
- Windows' own settings for snapping, shaking to minimise, scroll bars and animation effects on one page

### Games and presets

- HDR switched on for an HDR game and off afterwards
- monitor brightness, contrast and input changed over DDC/CI, and a second monitor turned off while you play
- a "couch" template: when the TV interface opens, sound and the main screen move to the TV and the desk monitors go dark
- presets on a gamepad button combination
- tray icons shown or hidden per preset
- a game goes quieter while it's not in front, and comes back when you return to it
- streaming mode: the island, dock, widgets and cards never appear in a stream, recording or screen share
- whole-number scaling for old games in small windows, with sharp pixels
- care for OLED screens: the program's own bars shift by a pixel over time, and an idle OLED dims while you play on another screen

### For developers

- a look for the terminal in the program's colours
- open a terminal in the folder you're looking at, copy the path, open it in an editor
- which process holds a port, your own running servers, which process holds a file
- an editor for PATH and environment variables, with history and undo
- the PC stays awake while a build runs, and you hear when it's done
- a PowerShell module with suggestions from history, one search across every shell's history, short aliases for cmd and PowerShell
- project tasks as buttons, scheduled commands, a reminder of uncommitted and unpushed work
- how much space build folders and package caches take, with a way to clear them
- the Linux subsystem's memory and containers' ports
- SSH hosts in one click
- clipboard tools: format JSON, decode a token, base64, URL encoding, Unix time, a new GUID
- a different border colour for windows whose title mentions production or another word you pick
- developer switches for Windows in one place: file extensions, hidden files, full path in Explorer

### The window itself

- a new "Right now" page with what the program is doing at the moment
- the menu grouped into Appearance, Screens and windows, and Work
- search that finds pages, settings and commands, and runs them
- help in three parts and a tour that follows what you're interested in
- works with high-contrast themes, the keyboard alone and screen readers
- smoother, spring-based motion throughout the window
- after a preset first works, the program asks once for a Steam review

### Steam

- 68 achievements, up from 20
- Steam Workshop, open to copies bought on the account or shared through Steam Families
- uninstalling through Steam puts back everything the program changed: autostart, terminal and shell settings, icons, colours, the desk's look
- every new text in all 30 languages Steam supports

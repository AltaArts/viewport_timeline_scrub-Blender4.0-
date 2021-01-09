# Scrub timeline (Viewport scrub)

Scrub timeline in viewport and snap to nearest keyframe


/!\ Work in progress, under active development.
This is a standalone feature for later integration in Grease Pencil Tools

**[Download latest](https://github.com/Pullusb/viewport_timeline_scrub/archive/master.zip)**

<!-- ### [Demo Youtube]() -->

---  

## Description

Pop-up a timeline in viewport so you can scrub full screen

![Viewport scrubbing in time](https://github.com/Pullusb/images_repo/raw/master/Bl_scrub_timeline_preview.gif)

**Viewport timeline** : `F5` (temporary default shortcut)

Use addon preference to customize shortcut, Display colors and fetaures

Use designated shortcut in viewport to call temporary timeline and scrub

While scrubbing use `Ctrl` key or `RMB` (Right click) to snap to nearest keyframe

---

### TODO

- Better way for user to chose keymap live in preferences

- Improve drawing performance

HUD
- add source frame as text ? (draw depending on timeline HUD placement)
- display marks for start and end ?
- display marks for keyframes ?



<!-- - question
Most important:
for the shortcut:
    use a "on press" key without pressing mouse, (currently used)
    use shortcut + mouse press ? (complex do right clic + left clic press with a tablet pen...)

Currently use only GP keys:
  Does it need to have a separate "mode" for GP keys and Objects keys

Other:
Should it disable onion skin like normal scrubbing does
Should it pause playback launched during play (and keep stop after) ?
Snap on key by default ?

- drawbacks
add an undo step containing timeline move. If not, a ctrl+Z after a new stroke move back timeline)

-- ideas
- Use also in other editors with a per editor behavior (difficult to find a cross editor shortcuts):
  - on 3D view (active layer key only)
  - on GP dopesheet : all layers keys (or only active same as above)
  - on object dopesheet : considering all object keys

Done:
- OK vertical thin line for current position
- OK snap to showed keyframe
- OK show text
- OK prefs to customize color appeareance
- OK add frame offset value as text
- OK prefs conditions to activate only parts of HUD
-->

<!-- allowed_key = ('NONE', 'LEFTMOUSE', 'MIDDLEMOUSE', 'RIGHTMOUSE', 'BUTTON4MOUSE', 'BUTTON5MOUSE', 'BUTTON6MOUSE', 'BUTTON7MOUSE', 'PEN', 'ERASER', 'MOUSEMOVE', 'INBETWEEN_MOUSEMOVE', 'TRACKPADPAN', 'TRACKPADZOOM', 'MOUSEROTATE', 'MOUSESMARTZOOM', 'WHEELUPMOUSE', 'WHEELDOWNMOUSE', 'WHEELINMOUSE', 'WHEELOUTMOUSE', 'EVT_TWEAK_L', 'EVT_TWEAK_M', 'EVT_TWEAK_R', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', 'ZERO', 'ONE', 'TWO', 'THREE', 'FOUR', 'FIVE', 'SIX', 'SEVEN', 'EIGHT', 'NINE', 'LEFT_CTRL', 'LEFT_ALT', 'LEFT_SHIFT', 'RIGHT_ALT', 'RIGHT_CTRL', 'RIGHT_SHIFT', 'OSKEY', 'APP', 'GRLESS', 'ESC', 'TAB', 'RET', 'SPACE', 'LINE_FEED', 'BACK_SPACE', 'DEL', 'SEMI_COLON', 'PERIOD', 'COMMA', 'QUOTE', 'ACCENT_GRAVE', 'MINUS', 'PLUS', 'SLASH', 'BACK_SLASH', 'EQUAL', 'LEFT_BRACKET', 'RIGHT_BRACKET', 'LEFT_ARROW', 'DOWN_ARROW', 'RIGHT_ARROW', 'UP_ARROW', 'NUMPAD_2', 'NUMPAD_4', 'NUMPAD_6', 'NUMPAD_8', 'NUMPAD_1', 'NUMPAD_3', 'NUMPAD_5', 'NUMPAD_7', 'NUMPAD_9', 'NUMPAD_PERIOD', 'NUMPAD_SLASH', 'NUMPAD_ASTERIX', 'NUMPAD_0', 'NUMPAD_MINUS', 'NUMPAD_ENTER', 'NUMPAD_PLUS', 'F1', 'F2', 'F3', 'F4', 'F5', 'F6', 'F7', 'F8', 'F9', 'F10', 'F11', 'F12', 'F13', 'F14', 'F15', 'F16', 'F17', 'F18', 'F19', 'F20', 'F21', 'F22', 'F23', 'F24', 'PAUSE', 'INSERT', 'HOME', 'PAGE_UP', 'PAGE_DOWN', 'END', 'MEDIA_PLAY', 'MEDIA_STOP', 'MEDIA_FIRST', 'MEDIA_LAST', 'TEXTINPUT', 'WINDOW_DEACTIVATE', 'TIMER', 'TIMER0', 'TIMER1', 'TIMER2', 'TIMER_JOBS', 'TIMER_AUTOSAVE', 'TIMER_REPORT', 'TIMERREGION', 'NDOF_MOTION', 'NDOF_BUTTON_MENU', 'NDOF_BUTTON_FIT', 'NDOF_BUTTON_TOP', 'NDOF_BUTTON_BOTTOM', 'NDOF_BUTTON_LEFT', 'NDOF_BUTTON_RIGHT', 'NDOF_BUTTON_FRONT', 'NDOF_BUTTON_BACK', 'NDOF_BUTTON_ISO1', 'NDOF_BUTTON_ISO2', 'NDOF_BUTTON_ROLL_CW', 'NDOF_BUTTON_ROLL_CCW', 'NDOF_BUTTON_SPIN_CW', 'NDOF_BUTTON_SPIN_CCW', 'NDOF_BUTTON_TILT_CW', 'NDOF_BUTTON_TILT_CCW', 'NDOF_BUTTON_ROTATE', 'NDOF_BUTTON_PANZOOM', 'NDOF_BUTTON_DOMINANT', 'NDOF_BUTTON_PLUS', 'NDOF_BUTTON_MINUS', 'NDOF_BUTTON_ESC', 'NDOF_BUTTON_ALT', 'NDOF_BUTTON_SHIFT', 'NDOF_BUTTON_CTRL', 'NDOF_BUTTON_1', 'NDOF_BUTTON_2', 'NDOF_BUTTON_3', 'NDOF_BUTTON_4', 'NDOF_BUTTON_5', 'NDOF_BUTTON_6', 'NDOF_BUTTON_7', 'NDOF_BUTTON_8', 'NDOF_BUTTON_9', 'NDOF_BUTTON_10', 'NDOF_BUTTON_A', 'NDOF_BUTTON_B', 'NDOF_BUTTON_C', 'ACTIONZONE_AREA', 'ACTIONZONE_REGION', 'ACTIONZONE_FULLSCREEN') -->


## Changelog:

0.4.3:

- feat: Display keyframes on timeline

- fixing some problem with onion skin auto hide

- better readme with demo gif

0.4.2:

- fix: display HUD/OSD only in active viewport

- fix: non blocking error with an uninitialized frame variable

- disable onion skin during the modal

0.4.1:

- fix: corrected an offset bug in time when viewport used was not leftmost in screen

0.4.0:

- Base text overlay dpi according to user settings

- Snap mode on left click + continuous press

0.3.0:

- initial commit
# fluent-dark-grey
### This is a fork of dogeshep's Fluent Dark theme for OBS Studio, altered to resemble the native Grey theme. Some additional fixes were also applied.

![Fluent Dark Grey Preview](https://github.com/Pigney/fluent-dark-grey/assets/34039700/34fe8cc0-e313-4d3f-a067-430564d3ffae)
### Also included is a .reg file for dark Windows Titlebars as seen in the screenshot. This can be deleted after it has been run.

Installation:\
Unzip the Zip file into the following folder:\
Windows: %APPDATA%\obs-studio\themes\ \
macOS: ~/Library/Application Support/obs-studio/themes/\
Linux: ~/.config/obs-studio/themes/\
Restart OBS Studio\
Go to Settings > General and select 'Fluent Dark (Grey)' in the Themes dropdown.

List of changes:
```
remove "qproperty-peakDecayRate: 23.4;" to prevent forced Fast decay rate.
change "qproperty-foregroundErrorColor:" to "rgb(255, 64, 64);"
change "OBSTheme {highlight:" to "rgb(152, 152, 152);"
change "QPushButton:checked {background-color:" to "rgb(152, 152, 152);"
change "QSlider::groove:vertical {background-color:" to "rgb(54, 54, 54);"
add "* [themeID="filtersIcon"] {qproperty-icon: url(./Fluent Dark Grey/filter.svg);}" to fix dark filter icon.
replaced unlocked.svg, locked.svg, visible.svg, hidden.svg and ./settings/general.svg with icons from Dark & Light to improve visibility.
changed "OBSQTDisplay {qproperty-displayBackgroundColor:" to "rgb(46, 46, 46);"
increased size of mute.svg to improve visibility.
created unassigned.svg and added "MuteCheckBox::indicator:indeterminate {image: url(./Fluent Dark Grey/unassigned.svg);}" for parity with latest OBS icons.
modify ./settings/audio.svg to be more consistent with other audio icons.
modify ./settings/stream.svg & ./settings/general.svg to improve visibility.
remove "margin-right: 8px;" from "QPushButton#sourceFiltersButton" & "QPushButton#sourcePropertiesButton"
changed ./checkbox/checkbox_checked.svg, ./checkbox/checkbox_checked_focus.svg and ./checkbox/checkbox_checked_pressed.svg to grey.
centered ./sources/microphone.svg, ./sources/default.svg & ./sources/media.svg
added "min-height: 16px;" to "#stackedMixerArea QPushButton" & "OBSBasicFilters #widget QPushButton, OBSBasicFilters #widget_2 QPushButton"
changed color of Controls buttons to grey.
changed "* [themeID="error"] {color:" to "rgb(230,0,0);"
changed "OBSHotkeyLabel[hotkeyPairHover=true] {color:" to "rgb(180,180,180);"
changed "*[gridMode="true"] SceneTree::item:hover:!pressed:selected, *[gridMode="false"] SceneTree::item:hover:!pressed:selected {background-color:" to "rgb(200, 200, 200);"
```

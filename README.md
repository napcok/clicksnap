# clicksnap

clicksnap for Openbox - click on the appropriate area of the window to snap it in a given direction. 
Works with active and inactive windows.
Configurable gap between windows.

*(Far from perfection, but imho already enough good to use)*

See it in action: https://www.youtube.com/watch?v=UzgUYYXnRww

## Requirements
- wmctrl
- xdotool
- xwininfo

## Installation
  
Add this mousebind action to context Frame:

      <mousebind action="Press" button="C-Left">
        <action name="UnmaximizeFull"/>
        <action name="Execute">
          <command>clicksnap</command>
        </action>
      </mousebind>


## Usage
clicksnap is binded to <kbd>Ctrl</kbd> + <kbd>Left Mouse Click</kbd>
Click inside window you like to move.
There are 9 areas ... see screenshot :)

![clicksnap](clicksnap.png "clicksnap areas")

## Configuration

Edit variables on top of script

    ### Configuration
    # Gap between windows
    GAP="32"
    show_outer_gap="true"
    # TITLEBAR HEIGHT - no idea how to find it from cli 
    TITLEBAR_HEIGHT="20"
    # Activate moved windows?
    activate_window="false"
    ### End Configuration

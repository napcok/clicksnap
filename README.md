# clicksnap

clicksnap for Openbox - click on the appropriate area of the window to snap it in a given direction. 
Works with active and inactive windows.

*(Far from perfection, but imho already enough good to use)*

## Requirements
- wmctrl
- xdotool

## Installation
    wget https://git.maboxlinux.org/napcok/clicksnap/raw/branch/master/clicksnap
    chmod +x clicksnap

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

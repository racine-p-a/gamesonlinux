# Call of duty

## Installation

The steam version works using these launch options : `__GL_ExtensionStringVersion=17700 %command% +set r_ignorehwgamma 1__GL_ExtensionStringVersion=17700 %command% +set r_ignorehwgamma 1`

## Problems

### Mouse lag

If your mouse input behaves strangely, you must force the game to display the native resolution of your screen.

To achieve this, go to your game files `/path/to/steamapps/common/Call of Duty/Main` and open the `config.cfg` file with
your preferred text editor.

In a case of a 1920*1080 screen, change those values :

- seta r_customwidth "1920"
- seta r_customheight "1080"
- seta cg_fov "96"
- seta r_mode "-1"
- seta com_introplayed "1"
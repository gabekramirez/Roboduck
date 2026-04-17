# Roboduck

In Roboduck you play as a bread-tossing toaster robot exploring the local park, feeding ducks, and avoiding obstacles.
- By pressing the respective buttons (A and D by default), you move left and right on screen.
- You can aim and click to throw bread; if the bread hits a duck, you will gain points.
- Bread that is thrown offscreen can't be collected by the player.
- You can collect loaves and other collectibles to add to your bread ammo count.
- Ducks will walk around randomly, making them harder to hit.
- Obstacles (trees, lily pads, buildings, etc.) will end the game when hit by the player.


Table of Contents

=================

* [Windows Installation](#windows-installation)


## Windows Installation

Building Roboduck for Windows requires [Python](https://www.python.org/), [Pygame](https://www.pygame.org/docs/), and [PyInstaller](https://pyinstaller.org/en/stable/).

Once you have Python and its package manager pip downloaded and installed, Pygame and PyInstaller can be installed with:

```shell

pip install pygame

pip install pyinstaller

```

Then you can build Roboduck using:

```shell
git clone https://github.com/gabekramirez/roboduck.git
pyinstaller main.py -w -n Roboduck -i assets\\roboduckicon.ico -F --add-data assets:assets

```

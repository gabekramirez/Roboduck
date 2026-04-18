# Roboduck

This is a video game that I developed back for FBLA's High School Competitive Events back in 2022. The code is a bit of a mess, and I would write it much differently if I were to create a game like this nowadays, however the game itself is fully complete and functional. And that is my intended purpose with this project. To demonstrate something fully complete and functional.

If you want to try out Roboduck without having to build it yourself, consider checking out the game on [itch.io](https://gabekramirez.itch.io/roboduck)


Table of Contents
=================
- [Gameplay](#gameplay)
- [Windows Build](#windows-build)
- [Web Build](#web-build)


## Gameplay

In Roboduck you play as a bread-tossing toaster robot exploring the local park, feeding ducks, and avoiding obstacles.
- By pressing the respective buttons (A and D by default), you move left and right on screen.
- You can aim and click to throw bread; if the bread hits a duck, you will gain points.
- Bread that is thrown offscreen can't be collected by the player.
- You can collect loaves and other collectibles to add to your bread ammo count.
- Ducks will walk around randomly, making them harder to hit.
- Obstacles (trees, lily pads, buildings, etc.) will end the game when hit by the player.


## Windows Build

Building Roboduck for Windows requires [Python](https://www.python.org/), [Pygame](https://www.pygame.org/docs/), and [PyInstaller](https://pyinstaller.org/en/stable/).

Once you have Python and its package manager pip downloaded and installed, Pygame and PyInstaller can be installed with:

```shell
pip install pygame
pip install pyinstaller
```

Then you can build Roboduck.exe using:

```shell
git clone https://github.com/gabekramirez/roboduck.git
cd roboduck
pyinstaller main.py -w -n Roboduck -i assets\\roboduckicon.ico -F --add-data assets:assets
```


## Web Build

Building Roboduck for the web requires [Python](https://www.python.org/), [Pygame](https://www.pygame.org/docs/), and [Pygbag](https://pypi.org/project/pygbag/).

Once you have Python and its package manager pip downloaded and installed, Pygame and Pygbag can be installed with:

```shell
pip install pygame
pip install pygbag
```

Then you can build and run Roboduck for the web using:

```shell
git clone https://github.com/gabekramirez/Roboduck.git
pygbag roboduck
```

This works, but it is recommended for the web build, however, that you first edit line 11 in main.py to ```IS_WEB = True``` before running pygbag.

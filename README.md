# tmux-spotify
A little script that is based heavily on a script from https://github.com/wandernauta

## Use Case
This is to be used in your tmux status line. If you want full terminal access you will want to use Wander script for
that. If can be found https://gist.githubusercontent.com/wandernauta/6800547/raw/db881a9100eb9b1e684c99962bde086a47ebcf08/sp

## Configuration
There is one configuration option in the bash script. If you open it in your text editor, there is a variable on the top called `CHAR_LENGTH`. This variable will trim the song title if its too long.

## Install
Download or clone this repo and copy the tmux-spotify file to a location in your PATH so tmux can access it. Then you will want to edit your tmux.conf and set the following

```
set -g status-right $(tmux-spotify both)
```
This will display a ♫, the artist, and the title of the song

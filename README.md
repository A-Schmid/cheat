# Quick Cheatsheet Access

I was really annoyed that I'm always searching for the same things, such as data sheets for parts I often use, pinout diagrams for microcontrollers, or how to do a certain thing with some python library.
Therefore, I created a little script that lets me quickly access such documents on my machine.

## How it works

The documents of interest are stored in a directory on my system (`~/cheat/`).
The script (bound to a keybinding of course) uses [dmenu](https://tools.suckless.org/dmenu/) to browse through this directory's content.
By naming the documents with searchability in mind (e.g. `TSOP382 infrared IR receiver datasheet.pdf`), dmenu can easily find the desired document with a pretty short query.
Even if we're not sure how the document is called exactly, we can browse through a selection by using a more general query (in this case *datasheet* or *infrared*).

Of course, it is not required to use dmenu - I'm sure similar programs like fzf could also be used for this workflow.

### Recommended Programs

Currently, my cheatsheet directory only contains PDF and image files.
For viewing PDF's, I strongly recommend [zathura](https://pwmt.org/projects/zathura/) as it opens so quicky.
As my default PDF viewer is a different program, zathura is called explicitly by the script.

For images, [sxiv](https://wiki.archlinux.org/title/Sxiv) is a good option.

In case I incorporate different file types (e.g. websites?), this list will be extended.

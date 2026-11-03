# For creators

Everything Stillward Display can wear is a file somebody can make: window
animation styles, taskbar looks, pointer sets, widgets, icon sets, island
activities and setups. None of them is code. The program checks every file
against its format before it uses it, brings each number into its range, and
refuses a field it does not know with the reason.

You can make all of them in the program itself, where each library has an
editor, and publish them to the Steam Workshop from there. The files below are
for making them by hand or from a script.

## The formats

| Kind | File | Schema |
|---|---|---|
| Window animation style | `*.motion.json`, up to 64 KB | [`schema/motion.json`](schema/motion.json) |
| Taskbar look | `*.taskbar.json`, up to 16 KB | [`schema/taskbar.json`](schema/taskbar.json) |
| Widget | `*.widget.json`, up to 64 KB, 64 items, 8 pictures | [`schema/widget.json`](schema/widget.json) |
| Pointer set | `scheme.json` beside its pointers | [`schema/pointers.json`](schema/pointers.json) |
| Pointer studio document | `studio.json` beside a set's `scheme.json` | [`schema/pointer-studio.json`](schema/pointer-studio.json) |
| Icon set | a folder of drawings and its description | [`schema/icons.json`](schema/icons.json) |
| Island activity | a widget's items for the island's two forms | [`schema/activity.json`](schema/activity.json) |
| Setup | the items it wears, by Workshop number | [`schema/setup.json`](schema/setup.json) |

Each schema is also served at `https://stillwarddisplay.com/schema/<name>.json`,
and a file the program saves starts with that `$schema` line. An editor that
understands JSON Schema then offers every field with its range and meaning as
you type. The copies here are the same files as on the site and change in the
same release.

## Examples and templates

In [`examples/`](examples/):

- `lamp.motion.json`: a minimize shape with sliders an author can expose
- `jelly.motion.json`: a drag
- `corner-first.motion.json`: a mesh, the corner nearest the button leading
- `quiet-oled.taskbar.json`: a taskbar look
- `clock.widget.json`: a widget
- `stillward-pointer-template.zip`: seventeen pointers to draw over
- `stillward-icon-set.zip`: an icon set to start from

## A first style in five minutes

1. Open the Animations page and stay on **Minimize**. Choose **Make a style**.
2. Set **Effect** to **Grid** and choose the middle key moment on the track.
3. Drag the bottom row of points toward the taskbar button and the top row a
   little to one side. The picture above plays it.
4. Choose **Add a key** and pull that moment's grid into a narrower shape. Turn
   on **Slow motion** and minimize a window to see it on the desk.
5. Name it, add a line of description and **Save**. In your styles it now has
   **Publish**, and the editor has **Save as a file**.

## Editing by hand

On the Animations page, **Open a style from a file** adds it and chooses it.
While Stillward runs, every save to that file updates the style, so the loop is:
save in your editor, minimize a window. Dropped on the window, a
`.motion.json` or `.taskbar.json` file joins the library the same way a
Workshop item does.

The program checks a file from the command line without opening a window,
starting Steam or counting time. It ends with code 0 for a file it takes and 1
for one it refuses:

```
stillward-display.exe --check "Calm.motion.json" --gif "Calm.gif"
```

The program is in its folder in your Steam library.

## What a file cannot do

A style cannot run anything, open a file, reach the network or read the screen.
The program moves pictures of windows that Windows already draws and never
draws inside another program. A file made to be extreme still draws something
sane, and one from a newer version is refused whole, so it never half works.

## Licence

The files in this folder are [CC0](https://creativecommons.org/publicdomain/zero/1.0/):
copy them, change them, publish what you make from them, no credit needed.

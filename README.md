# Notion for Linux
Nativefier-based wrapper to let notion function like a native app on linux.

## What is this
This is a small repo that just contains the output of running [Nativefier](https://github.com/jiahaog/nativefier) on [Notion](https://www.notion.so/).

## Why
Notion has a desktop client for Windows and Mac, but no love for Linux. There are a few other electron-based projects looking at wrapping it, but they all had small things I didn't like about them.

## How do I install it
- unzip the `notion-linux-x64.zip` somewhere
- copy the `notion-linux-x64` folder to somewhere you keep applications (I put mine in `/opt/`)
- copy the notion.desktop file somewhere you keep application manifests (I put mine in `/usr/share/applications/` but you might want to put it somewhere else maybe. More info [here.](https://developer.gnome.org/integration-guide/stable/desktop-files.html.en))
- change the paths in the desktop file if you put your `notion-linux-x64` folder somewhere else.

## How did you make this
- install nativefier
- run this command:

`nativefier "https://www.notion.so" --name "Notion" -i /opt/notion-linux-x64/logo.png --internal-urls ".?(notion.so).?"`

## Is this in any way official?
Definitely not. If Notion release a desktop client start using that instead of this.

Pellucid
===================

Pellucid is a skin for Kodi Media Centre (Kodi 21 Omega).

This is a maintained fork of [chrisbevan/skin.pellucid](https://github.com/chrisbevan/skin.pellucid), updated for Kodi 21 Omega compatibility while preserving the full feature set including home screen menu editing via Skin Shortcuts.

Built for the living room, Pellucid is a clean and carefully designed Kodi experience designed for maximum usability and minimum fuss.

![Pellucid home screen](resources/screenshot-01.jpg)

#### Features

- Full home screen menu customization via Skin Shortcuts
- Full PVR / Live TV support
- Video Versions and Video Extras support (new in Omega)

#### Requirements

- Kodi 21 (Omega)
- [script.skinshortcuts](https://github.com/MikeSiLVO/script.skinshortcuts) v2.0.3+ (MikeSiLVO's maintained fork -- not available in the official Kodi addon repo)

#### Installing Skin Shortcuts

Pellucid needs the Skin Shortcuts add-on, which is not in the official Kodi
repo:

1. Download the latest release zip from
   [MikeSiLVO/script.skinshortcuts](https://github.com/MikeSiLVO/script.skinshortcuts/releases)
2. In Kodi: **Settings > Add-ons > Install from zip file** and select the
   downloaded zip

#### Installing Pellucid

This fork has no release zips, so install it straight from git -- clone it into
your Kodi add-ons directory, making sure the folder is named exactly
`skin.pellucid`:

```bash
git clone https://github.com/vadikmironov/skin.pellucid.git \
    ~/.kodi/addons/skin.pellucid
```

Restart Kodi, then select Pellucid under **Settings > Interface > Skin**. To
update later:

```bash
cd ~/.kodi/addons/skin.pellucid && git pull
```

(Prefer a zip? GitHub's **Code > Download ZIP** works too, but rename the
extracted `skin.pellucid-master` folder to `skin.pellucid` first.)

#### Editing the home menu

Edit any menu (home, video, music, pictures, games) from the **Menus**
section of the skin settings, which opens the Skin Shortcuts editor. Your
changes are saved by Skin Shortcuts and take effect on the next skin reload.

For stability on Kodi 21 Omega, Pellucid builds the menu **once per install**
(at first startup) rather than on every return to the home screen -- the old
per-visit rebuild could spawn overlapping Skin Shortcuts processes and crash
Kodi under Python 3.12. If the menu ever goes missing or out of sync, use the
**Rebuild home menu** button in the Menus settings to force a one-shot rebuild.

#### Screenshots

| Library | Info dialog |
|---------|-------------|
| ![Movies library](resources/screenshot-03.jpg) | ![Movie info](resources/screenshot-02.jpg) |

#### Credits

- Original skin created by theDeadManInYossariansTent
- Additional homescreen wallpapers by [Dadebue](https://www.instagram.com/dadebue/)
- Discussion thread: http://forum.kodi.tv/forumdisplay.php?fid=267

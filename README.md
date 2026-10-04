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
- [script.skinshortcuts](https://github.com/MikeSiLVO/script.skinshortcuts)
  **2.0.3** -- a hard dependency on the 2.x line. Skin Shortcuts 3.x is a
  complete rewrite that does not work with Pellucid's menus; a port of
  Pellucid to 3.x is work in progress.

#### Installing Skin Shortcuts

Pellucid needs Skin Shortcuts 2.0.3, the version in Kodi 21's official add-on
repo. To install it from its release zip instead:

1. Download
   [script.skinshortcuts-2.0.3.zip](https://github.com/MikeSiLVO/script.skinshortcuts/releases/download/v2.0.3/script.skinshortcuts-2.0.3.zip)
   -- not the latest release, which is 3.x
2. In Kodi, turn on **Settings > System > Add-ons > Unknown sources**, then
   **Settings > Add-ons > Install from zip file** and select the downloaded
   zip

Kodi 22 (Piers)'s official repo carries Skin Shortcuts 3.x. Before upgrading
to Kodi 22, turn off its auto-update: **Settings > System > Add-ons > Manage
dependencies > Skin Shortcuts**, then select **Auto-update** until it shows
**Off**.

#### Installing Pellucid

Download `skin.pellucid-<version>.zip` from the
[latest release](https://github.com/vadikmironov/skin.pellucid/releases/latest).
In Kodi, turn on **Settings > System > Add-ons > Unknown sources** (Kodi only
installs zip files with it on), then **Settings > Add-ons > Install from zip
file**. If Skin Shortcuts is not installed yet, Kodi 21 installs 2.0.3 from its
official repo along with it. Then select Pellucid under
**Settings > Interface > Skin**.

To track the latest changes instead, install it from git -- clone it into your
Kodi add-ons directory, making sure the folder is named exactly
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

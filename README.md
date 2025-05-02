<h1 align="center">
  <b>shadPS4 Game Compatibility</b>
</h1>

<h2 align="center">
<a href="https://github.com/shadps4-emu/shadps4-game-compatibility/labels/status-playable">
    <img src="https://img.shields.io/github/issues-search/shadps4-emu/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-playable&style=for-the-badge&color=8BA503&label=Playable"/>
<a href="https://github.com/shadps4-emu/shadps4-game-compatibility/labels/status-ingame">
    <img src="https://img.shields.io/github/issues-search/shadps4-emu/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-ingame&style=for-the-badge&color=F3BB00&label=Ingame"/>
<a href="https://github.com/shadps4-emu/shadps4-game-compatibility/labels/status-menus">
    <img src="https://img.shields.io/github/issues-search/shadps4-emu/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-menus&style=for-the-badge&color=FF5C1A&label=Menus"/>
<a href="https://github.com/shadps4-emu/shadps4-game-compatibility/labels/status-boots">
    <img src="https://img.shields.io/github/issues-search/shadps4-emu/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-boots&style=for-the-badge&color=A7001E&label=Boots"/>
<a href="https://github.com/shadps4-emu/shadps4-game-compatibility/labels/status-nothing">
<img src="https://img.shields.io/github/issues-search/shadps4-emu/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-nothing&style=for-the-badge&color=black&label=Nothing"/>
</h2>

- **status-playable**: Games that can be run without any issues.
- **status-ingame**: Games that can reach gameplay but have issues.
- **status-menus**: Games that can reach the menu but freeze/crash when trying to proceed further.
- **status-boots**: Games that show any visual/audio output but freeze/crash before reaching the menu.
- **status-nothing**: Games that crash when trying to launch or only show a black screen.

## Rules:

**Major Releases Only**
- Only publish results from major [**shadPS4 releases**](https://github.com/shadps4-emu/shadPS4/releases/latest) (e.g. v0.8.0).

**Insert All Necessary Information**
- Make sure you put all the necessary information: **Title**, **Game ID**, **Game Version**, **Emulator Version**, **Compatibility Status** and **Operating System**.

**Report a game only once, except...**
- ...when the OS is different, we allow one report per system-OS (Windows, Linux and macOS). So duplicate entries can exist if they are for different OS.
- ...if the CUSA is different (e.g. Bloodborne = CUSA00900 & CUSA03173)

**Do not report a game with a already existing entry with the same CUSA and OS**
- If the CUSA and OS is the same as an older report, comment on the older report with the game's new status, a description of how it behaved, any screenshots you took, and a log.

**Unmodified Game Dumps**
- Only publish reports with unmodified game dumps. If any patches or modifications are applied, the report will be removed. Repackaging your dumps to FPKGs will be treated the same way.
- Piracy of any form is strictly prohibited. Any reports involving pirated game dumps will be removed, and reporters suspected of piracy will be blocked from the shadPS4 repository.

**Dump your PlayStation 4's system files before reporting**
- Some PlayStation 4 firmware libraries are required for games to behave properly. Details about the required modules are listed in the information section.

**Use the comment section only for reporting changes on a new release**
- This isn't a place for discussion or support requests. Only comment when you want to report about new major releases, any off-topic comments will be deleted.
- When updating a report, do it by providing a log. Comments reporting changes without a log will not be considered. If you're updating your own post on a new release, do it by adding a comment with your log rather than editing your original post. This way it will be easier for us to know if there was an update in your report.

## Information:

shadPS4 can load some PlayStation 4 firmware files, these must be dumped from your legally owned PlayStation 4 console.\
The following firmware modules are supported and must be placed in shadPS4's `user/sys_modules` folder.

<div align="center">

| Modules                 | Modules                 | Modules                 | Modules                 |  
|-------------------------|-------------------------|-------------------------|-------------------------|  
| libSceCesCs.sprx        | libSceFont.sprx         | libSceFontFt.sprx       | libSceFreeTypeOt.sprx   |
| libSceJson.sprx         | libSceJson2.sprx        | libSceLibcInternal.sprx | libSceNgs2.sprx         |  
| libSceRtc.sprx          | libSceUlt.sprx          |                         |                         |  

</div>

> [!Caution]
> The above modules are required to run the games properly and must be extracted from your PlayStation 4.\
> **We do not provide any information or support on how to do this**.

<h1 align="center">
  <b>shadPS4 Game Compatibility</b>
</h1>

<h2 align="center">
<a href="https://github.com/shadps4-compatibility/shadps4-game-compatibility/labels/status-playable">
    <img src="https://img.shields.io/github/issues-search/shadps4-compatibility/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-playable&style=for-the-badge&color=8BA503&label=Playable"/>
<a href="https://github.com/shadps4-compatibility/shadps4-game-compatibility/labels/status-ingame">
    <img src="https://img.shields.io/github/issues-search/shadps4-compatibility/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-ingame&style=for-the-badge&color=F3BB00&label=Ingame"/>
<a href="https://github.com/shadps4-compatibility/shadps4-game-compatibility/labels/status-menus">
    <img src="https://img.shields.io/github/issues-search/shadps4-compatibility/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-menus&style=for-the-badge&color=FF5C1A&label=Menus"/>
<a href="https://github.com/shadps4-compatibility/shadps4-game-compatibility/labels/status-boots">
    <img src="https://img.shields.io/github/issues-search/shadps4-compatibility/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-boots&style=for-the-badge&color=A7001E&label=Boots"/>
<a href="https://github.com/shadps4-compatibility/shadps4-game-compatibility/labels/status-nothing">
<img src="https://img.shields.io/github/issues-search/shadps4-compatibility/shadps4-game-compatibility?query=is%3Aopen+label%3Astatus-nothing&style=for-the-badge&color=black&label=Nothing"/>
</h2>

- **status-playable**: Games that can be played without any major issue.
- **status-ingame**: Games that can reach gameplay but have issues.
- **status-menus**: Games that can reach the menu but freeze/crash when trying to proceed further.
- **status-boots**: Games that show visual or audio output but freeze or crash before reaching the menu.
- **status-nothing**: Games that crash when trying to launch or hang on a black screen.

## Rules:

**Major Releases Only**
- Only publish results from major [**shadPS4 releases**](https://github.com/shadps4-emu/shadPS4/releases/latest) (e.g. v0.12.5).

**Insert All Necessary Information**
- Make sure you put all the necessary information: **Title**, **Game ID**, **Game Version**, **Emulator Version**, **Compatibility Status** and **Operating System**.

**Report a game only once, except...**
- ...when the OS is different, we allow one report per system-OS (Windows, Linux and macOS). So duplicate entries can exist if they are for different OS.
- ...if the CUSA is different (e.g. Bloodborne = CUSA00900 & CUSA03173)

**Do not report a game with an already existing entry with the same CUSA and OS**
- If the CUSA and OS is the same as an older report, comment on the older report with the game's new status, a description of how it behaved, any screenshots you took, and a log.

**Unmodified Game Dumps**
- Only publish reports with unmodified game dumps. If any patches or modifications are applied, the report will be removed. Repackaging your dumps to FPKGs will be treated the same way.
- Piracy of any form is strictly prohibited. Any reports involving pirated game dumps will be removed, and reporters suspected of piracy will be blocked from the shadPS4 repository.

**Don't change settings that can impact the game's behavior**
- Changing settings like "isPS4Pro", "isDevKitConsole", or the Vblank Frequency can change the way a game behaves, any reports with these settings modified will be closed.
- Some settings, like readbacks or direct memory access are permitted, and reports with them enabled will be tagged with the "experimental" tag for easy searching.

**Dump your PlayStation 4's system files before reporting**
- Some PlayStation 4 firmware libraries are required for games to behave properly. Details about the required modules are listed in the information section.

**Don't manually edit your log before posting it**
- Logs should be untouched, doing things such as trimming lines that are repeated over and over to make it more "readable" isn't something you should do, leave the log as is.
- In the rare case where the crash assert wouldn't show because the log file exceeds 100MB, using a log filter is allowed, but make sure to mention this in the report.

**Use the comment section only for reporting changes on a new release**
- This isn't a place for discussion or support requests. Only comment when you want to report about new major releases, any off-topic comments will be deleted.
- When updating a report, do it by providing a log. Comments reporting changes without a log will not be considered. If you're updating your own post on a new release, do it by adding a comment with your log rather than editing your original post. This way it will be easier for us to know if there was an update in your report.

## Information:

shadPS4 can load some PlayStation 4 firmware files, these must be dumped from your legally owned PlayStation 4 console.\
The following firmware modules are supported and must be placed in shadPS4's `sys_modules` folder.\
For more information on how to dump your firmware files, you can check the [shadPS4 wiki](https://github.com/shadps4-emu/shadPS4/wiki/I.-Quick-start-%5BUsers%5D#4-dumping-firmware-modules).

<div align="center">

| Modules                 | Modules                 | Modules                 | Modules                 |  
|-------------------------|-------------------------|-------------------------|-------------------------|  
| libSceCesCs.sprx        | libSceFont.sprx         | libSceFontFt.sprx       | libSceFreeTypeOt.sprx   |
| libSceJson.sprx         | libSceJson2.sprx        | libSceLibcInternal.sprx | libSceNgs2.sprx         |  
| libSceUlt.sprx          |                         |                         |                         |  

</div>

> [!Caution]
> The above modules are required to run the games properly and must be extracted from your PlayStation 4.

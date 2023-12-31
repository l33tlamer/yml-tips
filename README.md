<br>

Hello everyone,

**this post is to simply show a quick overview of popular editors that people might want to consider to edit their .yml (YML/YAML) files for use with PlexMetaManager (PMM).**

You should also consider giving our quick [YML Tutorial](https://metamanager.wiki/en/latest/home/guides/yaml.html) on the PMM Wiki a read to learn about quirks and features of YML.

A good editor can help a lot by assisting with having the **correct indent** for PMM (multiples of 2 spaces, no TAB stops, etc.), general checking of **YML structure** and warning of **possible errors**, even before you run the file through PMM. This can **save a lot of time** and avoid headaches, before having to troubleshoot within PMM. 

It can also display the code much more convient to make it nicer to work with and spot errors, or just to navigate around in a file by **highlighting certain things** and **coloring indents** etc.

Here is a quick example of how a config.yml from PMM can look like in standard Notepad versus how it can look like in VSCode:

![Screenshot of standard Notepad](/docs/assets/001.png)  
![Screenshot of VSCode](/docs/assets/002.png)

**A good choice of font** can also help by making it more distinct where a indent is correct and where it isnt.

For example, someone who is using **Wordpad** with the font *Times New Roman* to edit a PMM .yml will have a hard time to instantly spot a indent error, simply because a `i`will be the same width as a `X` and so on. Or three spaces might look like two. Even if you finally save the file as plaintext with the .yml extension, you will probably not spot such errors visually.

**So why make it harder on yourself, try a good editor instead.**

This is going to start with VSCode first, not because "*OMG <3 Microsoft!1*" but simply because its free and available on Windows, Mac and Linux.

# **Visual Studio Code (VS Code)**

*This one is quite popular but has a more "heavyweight" feel to it. However on a half decent computer it loads and reacts very well, its not like a Photoshop. But it might appear to be too much for some people if all they want to do is edit their .yml to add a Halloween collection for Plex. Even just the name might suggest that this is "for doing real programming" and not for simple things like editing a few config files. But dont let that scare you. Simply put, it can do a lot, but do you really need a lot?... Simple to install and use, shouldnt be confusing to most users.*

*The font and syntax color highlighting for PMM .yml should already work good by default. You can adjust font faces, sizes and more in the options.*

*Here is a example picture of how VSCode/VSCodium can look with the recommended extensions mentioned below:*

![Screenshot of VSCode with extensions](/docs/assets/003.png)

*By default it will already detect the indents being used in a (PMM .yml) file and adjust the use of TAB accordingly. This means pressing the TAB key will result in adding 2 spaces instead of a TAB-STOP or more/less spaces to make it work with PMM. The feature is called "**Editor: Detect Indentation**" and can be further adjusted in the Settings menu. So even if you´re the genius founder of Pied Piper and you care A LOT about [TABs and Spaces](https://www.youtube.com/watch?v=SsoOG6ZeyUI), you should be able to make it work.*

*And it is good idea to disable the option "Editor: Copy with Syntax Highlighting" because this can cause issues when you have trouble with PMM and you copy code from VSCode into your clipboard and you want to paste it  n Reddit or for example into the PMM Discord when looking for support.*

*You can find a summary of keyboard shortcuts [here](https://code.visualstudio.com/docs/getstarted/keybindings). If you have a large config.yml file for example you can press `CTRL + K + 0` to fold all sections, and `CTRL + K + J` to unfold them.*

*The "Product Telemetry" can be disabled under "File, Preferences, Telemetry Settings".*

**It is free and "opensource"**, made by Microsoft. Please see further down for **VSCodium** as alternative, and **recommended extensions** for both.

**Platforms:**

* Windows 8, 10 and 11 *(32bit x86, 64bit x64 and ARM)*

* Linux *(Debian, Ubuntu, RedHat, Fedora, etc. as 64bit x64, ARM and ARM64)*

* MacOS 10.11+ *(Universal, Intel CPU and Apple CPU)*

**Website: [https://code.visualstudio.com](https://code.visualstudio.com)**

# **VSCodium (VS Code alternative)**

*"Why does this exist? VSCodium is a community-driven, freely-licensed binary distribution of Microsoft’s editor VS Code. [...] Microsoft’s vscode source code is open source (MIT-licensed), but the product available for download (Visual Studio Code) is licensed under this not-FLOSS license and contains telemetry/tracking."*

*So if you want to use VSCode but youre not a fan of Telemetry/Tracking (even tho it can be disabled in VSCode), use this instead. Everything still works the same, there shouldnt be any issues.*

**It is also free and opensource**. Please see below for **recommended extenions**, and the quick tips above for VSCode also apply for VSCodium.

**Platforms:**

* Windows, Linux and Mac *(with some finer options than VSCode offers)*

**Website: [https://vscodium.com](https://vscodium.com)**

# **Code-Server (VS Code in your browser)**

*"Run VSCode on any machine anywhere and access it in the browser."*

*If you are into PMM and Plex, chances are you might also be into self-hosting other things. So a quick mention goes to VSCode running in a browser. Yes, the full application can be selfhosted and used from any browser, saving you from having to install it. In some setups this can be very useful, or it doesnt appeal to you at all. Not much more to say about this, everything that was said about VSCode/Codium should mostly apply to Code-Server too.*

*You could install it directly on a host, or run it in a container. A [Docker image](https://docs.linuxserver.io/images/docker-code-server) for example is provided by Linuxserver.io*

**Platforms:**

* Windows, Linux and Mac, wherever you can run the Docker image. Clients only need a half-modern browser to access.

**Website: [https://github.com/coder/code-server](https://github.com/coder/code-server)**

# VS Code extensions

These **extensions** are highly recommended and should work **VS Code, VSCodium and selfhosted Code-server**:

![Example GIF of YAML Language Support extensions](https://raw.githubusercontent.com/redhat-developer/vscode-yaml/main/images/demo.gif)

**[YAML Language Support](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)** by RedHat. *Detects errors in the YAML format, helps with autocomplete, etc.*

![Example screenshot of Indent-Rainbow extension](https://raw.githubusercontent.com/oderwat/vscode-indent-rainbow/master/assets/example.png)

**[indent-rainbow](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow)** by oderwat. *Colorizes the indentation and alternating the colors, making it very easy to see which indent refers to what etc.*

![Example screenshot of SSH_FS extension](https://raw.githubusercontent.com/SchoofsKelvin/vscode-sshfs/master/media/shell-tasks.png)

**[SSH_FS extension](https://open-vsx.org/extension/Kelvin/vscode-sshfs)** by Kelvin Schoofs. *Not directly YML-related, but if you dont run PMM directly on your computer, but on a NAS or a secondary computer etc, you might want to consider something like this. It allows you to mount the folder with your PMM config files directly into VSCode and work on them, without having to up/download them manually after each edit.*

You can simply access the **Extension Manager** in the left toolbar (or press `CTRL + SHIFT + X`) and then **search the marketplace** and install them.

# Notepad++

*This one is a modern classic. Very lightweight and as the name suggests a very much improved version of Windows Notepad. This also means it is only available for Windows platforms.*

![Screenshot of Notepad Plus Plus](https://notepad-plus-plus.org/assets/images/notepad4ever.png)

*Unfortunately there doesnt seem to be a plugin/feature as counterpart to "rainbow-indent", but you can make indentation more visible in Np++ atleast: In Settings, Style Configurator, Global Styles, Indent Guideline Style, you change the Foreground color to something more visible. This will change the color of the vertical line that shows the indentation, but it wont rotate between different colors like rainbow-indent does. Here is a example of what it can look like then:*

![Screenshot of Notepad Plus Plus styling](/docs/assets/004.png)

**Platforms:**

* Windows *(32bit x86, 64bit x64 and ARM64)*

**Website:** [https://notepad-plus-plus.org](https://notepad-plus-plus.org)

Recommended plugin:

* **[Auto Detect Indention](https://github.com/Chocobo1/nppAutoDetectIndent)**. *This will automatically detect the indent used when opening a existing file and adjust the use of TAB accordingly, so pressing TAB for PMM´s .yml files will not result in a actual TAB-STOP being added, but it will automatically do 2 spaces for each TAB press. A tiny feature that can make a big difference in every day use. For starting a fresh PMM .yml file, you can adjust the TAB size under Preferences, Language, Tab Settings, yaml and set it to 2 spaces.*

# Font

*Personally i have used the free "FiraCode" font for a long time and got very used to it, it works excellent for things like this. It should work with basically all editors and it comes with different variations and ligatures. More details are on the FiraCode GitHub page linked below. Whichever font you chose, it should be "monospace". That basically means every character is the same width, so a `x` takes up the same space as a `i` and the same as a empty space ` `, and as a result this keeps formatting in order.*

*To use a different font in VSCode/VSCodium, go to "File, Preferences, Settings". Under "Commonly Used" expand the "Text Editor" section and select Font. In the "Font Family" box enter the exact name of the font, such as "Fira Code". You can also chose a different variation of the font here if you enter "Fira Code Light" instead as the name, or "Fira Code Retina" which is optimized for high-resolution displays. And you can change the font size of course. If you want to enable the special ligatures that this font has, right below this there is a setting for "Font Ligatures" and you can click on "Edit in settings.json". It will open up the VSCode config file and the font ligature should already be selected. Change the option from "false" to "true" and save the file, then you can restart VSCode.*

**Website:** [https://github.com/tonsky/FiraCode](https://github.com/tonsky/FiraCode)

# Windows Terminal

*For Windows OS users when running PMM, having a much nicer to look at terminal can make a nice difference too. Also if it uses a  good monospace font, such as the above mentioned Fira Code. Here is a example of what you could make it look like:*

![Screenshot of Windows Terminal with theme](/docs/assets/005.jpg)

*This new and much improved app by Microsoft is a "all-in-one" for doing the classic Windows Command Prompt, Windows PowerShell and even the Microsoft Azure Shell. It can use various fonts, themes, optional always run as Admin, font anti-aliasing and so much more. If you also use VSCode to edit your YML, [there is a theme](https://github.com/cristipufu/windows-terminal-vscode-theme) to make the terminal have mostly the same look as VSCode. And there is a whole website dedicated to [Terminal themes](https://windowsterminalthemes.dev/).*

*Its available either from GitHub as a installer, or from the Windows10/11 builtin Windows Store as a app.*

**Website:** [https://github.com/microsoft/terminal](https://github.com/microsoft/terminal) (or [Windows Store](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701))

# Things to note

*Please not that these summaries are in no way meant to be exhaustive or a definitive source of knowledge. This is only a "quick" overview of alternatives that you could use to handle your YML files more easily, simply because we see a lot of PMM newcomers use things like Notepad or TextEdit and struggle a lot with simple things like formatting errors. There are of course many other editors around, like [SublimeText](https://www.sublimetext.com) for example. But we cant cover them all, and we wanted to keep this focused on the editors that are popular, well supported and maintained, and free to use. That leaves us with basically VS Code and NP++.*

For further questions, join our [Discord server](https://discord.gg/NfH6mGFuAB) or the subreddit at [/r/PlexMetaManager](https://www.reddit.com/r/PlexMetaManager/)

# EOF

<div align="center">

<img src="MinecraftServerManager/Assets/eclipse-256.png" alt="Eclipse logo" width="128" />

# Eclipse
### The Minecraft Server Manager

Create, run, and look after your Minecraft Java servers from one desktop app.

**Free to use · Ad-free · Built for Windows**

[Get started](#getting-started) · [Features](#features) · [FAQ](#faq) · [Support Eclipse](https://ko-fi.com/youssefs15)

</div>

---

## Your servers, in one place

Eclipse brings server creation, modpack imports, the console, player management, and world backups into a single interface. Start a vanilla world for friends or manage a modded server without juggling launch scripts and settings files.

Your server files stay on your PC, in folders you choose.

## Features

| | What you can do |
| --- | --- |
| **Create and import** | Create Vanilla, Paper, Fabric, Forge, or NeoForge servers. Import an existing server, a server-pack ZIP, or a supported modpack from CurseForge or Modrinth. |
| **Server dashboard** | Check server status and view CPU and memory usage graphs. View TPS when the server exposes supported tick information. |
| **Live console** | Read server output, send commands, and use the up and down arrow keys to browse command history. Respond to supported launcher confirmation prompts. |
| **Player management** | View online players and capacity. Send whispers, kick or ban players, manage the whitelist, and grant or remove operator permissions. |
| **World backups** | Create and restore compressed world backups, set a backup schedule and retention limit, and browse supported backup ZIPs created by server mods. |
| **Mods and updates** | Browse mods from Modrinth and CurseForge for compatible servers. Update supported server packs or change a vanilla server's version while preserving world and configuration data. |
| **Java and memory** | Select a Java runtime, install a supported runtime, or choose your own Java path. Adjust minimum and maximum RAM from Settings. |
| **File management** | Open a server's folder, move it to another location with progress feedback, or remove an instance. |
| **Connection details** | Reveal and copy local and public server addresses. Attempt automatic router forwarding through Online access on compatible networks. |
| **Personalisation** | Start with a dark theme and red accent, or choose light mode, system appearance, and your own accent colour. |

## Getting started

### 1. Download and launch

Open this repository's **Releases** section and download the Windows release. If it is supplied as a ZIP, extract it before opening **Eclipse.exe**.

Use a Windows PC with enough free disk space and memory for your chosen server. Internet access is needed for downloads and online browsing. Large modpacks can require considerably more resources than vanilla servers.

### 2. Add a server

Click **+ Add Instance** and choose how to begin:

- **Create server:** choose a name, folder, Minecraft version, server type, and RAM allocation.
- **Import existing server:** select the folder containing your existing server.
- **Server pack .zip:** import a server archive you already downloaded.
- **Modrinth / CurseForge:** browse modpacks and choose an available server version.

Accept the Minecraft EULA where prompted, then let the installation finish.

> **Choosing a folder:** an empty folder is used directly. A drive root or a folder that already contains files gets a new subfolder named after the server. Duplicate names receive a number, such as `My Server(1)`. The Create Server page previews the destination.

### 3. Start playing

Select your server and press **Start**. Eclipse opens its Console so you can follow startup.

Use **Settings** for everyday changes, including RAM and backups. Use **Advanced Settings** when you need to edit configuration text directly.

## Backups and updates

Eclipse's managed backups focus on **world data**, compressed into ZIP files. They are not complete copies of every mod, launcher, and configuration file.

- Create a backup before changing versions or updating a modpack.
- Set scheduled backups and the maximum backup count in the server's Settings.
- Keep Eclipse open for scheduled backups to run.
- Stop the server before restoring a backup.
- Keep a separate copy of important worlds outside the server's drive.

Preserving files during an update does not guarantee that an older world or configuration is compatible with the new version. Downgrades and major modpack changes need particular care.

## Connecting with friends

The address buttons keep addresses concealed until you reveal them.

| Who is connecting? | Address to use |
| --- | --- |
| Someone on your home network | The server PC's local address and server port |
| Someone outside your home network | Your public address and an externally reachable server port |

**Online access** can attempt to configure router forwarding and Windows Firewall. Router support varies, and CGNAT, double NAT, or ISP restrictions can prevent incoming connections. Eclipse does not verify connectivity from outside your network.

If automatic setup fails, you may need manual router configuration or another connection method. A public IP address alone does not make the server reachable.

## FAQ

### Is Eclipse free?

Yes. Eclipse is free to use and ad-free. Supporting development is optional.

### Do I need to install Java myself?

Eclipse can detect installed Java runtimes and download supported versions. You can also select a Java executable manually in the server's Settings. The required Java version depends on the Minecraft version and mod loader.

### Do I need API keys?

Public Modrinth browsing works without a token. CurseForge can use the application's default key when one is included in your build. You can provide your own credentials under **App Settings → Services**.

### Can every modpack run as a server?

No. Some packs are client-only or do not provide a usable server distribution. Available server downloads also depend on what the pack author publishes and what the provider permits.

### Where does Eclipse save its settings?

The server list and application data are stored under:

```text
%LOCALAPPDATA%\MinecraftServerManager
```

Server files remain in the folders you selected. Use **Open folder** beside a server's directory to find them.

### What happens when I delete a server?

Removing an instance from the manager and deleting its files are separate choices. **Delete from System** removes the server folder's contents but leaves the folder itself. Back up anything you want to keep first.

## Reporting a problem

Open an issue in this repository and include:

- Your Eclipse release and Windows version.
- The Minecraft version, loader, and modpack version, if applicable.
- What you were doing and what you expected to happen.
- Relevant console output or a screenshot.

Remove API keys, access tokens, public IP addresses, and other private details before posting.


## Support Eclipse

If Eclipse makes managing your servers easier, you can help fund maintenance, fixes, and future development.

<a href="https://ko-fi.com/youssefs15">
  <img src="MinecraftServerManager/Assets/KofiLogo.webp" alt="Support Eclipse on Ko-fi" width="48" />
</a>

**[Support Eclipse on Ko-fi](https://ko-fi.com/youssefs15)**

All app features remain available whether you contribute or not. You can also help by reporting bugs, testing releases, or sharing Eclipse with friends.

## Credits

- Built with [Avalonia](https://avaloniaui.net/) and [.NET](https://dotnet.microsoft.com/).
- Mod and modpack integrations with [Modrinth](https://modrinth.com/) and [CurseForge](https://www.curseforge.com/).
- Managed Java downloads provided through [Eclipse Adoptium](https://adoptium.net/).
- Interface icons from [Streamline Ultimate Bold Free](https://www.streamlinehq.com/icons/ultimate-bold-free).

Eclipse is an independent project and is not affiliated with or endorsed by Mojang or Microsoft. Mods and modpacks belong to their respective authors.

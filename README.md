### 📁 `INSTALL.md`

```markdown
# 🚀 Minecraft Server Installation on Debian in Proxmox CT

## Prerequisites:

1. A running Debian instance in Proxmox CT.
2. Root or sudo access to the instance.

## Installation Steps:

1. **Update and Upgrade**:
   ```bash
   apt update && apt upgrade -y
   ```

2. **Install Java**:
   ```bash
   apt install openjdk-17-jre-headless -y
   ```

3. **Create a Directory for Minecraft**:
   ```bash
   mkdir minecraft_server
   cd minecraft_server
   ```

4. **Download the Minecraft Server**:
   ```bash
   wget [URL_TO_MINECRAFT_SERVER.JAR]
   ```

5. **Start the Server**:
   ```bash
   java -Xmx1024M -Xms1024M -jar server.jar nogui
   ```

6. **Accept the EULA**:
   - Edit the `eula.txt` file and change `eula=false` to `eula=true`.

7. **Restart the Server**:
   ```bash
   java -Xmx1024M -Xms1024M -jar server.jar nogui
   ```

**Note**: Replace `[URL_TO_MINECRAFT_SERVER.JAR]` with the actual URL to download the Minecraft server jar file.
```

---

### 📁 `COMMANDS.md`

```markdown
# 🎮 Minecraft Server Commands Guide 🛠️

## 🖥️ Console Commands:

### Server Control:

1. **Starting the server**:
   ```bash
   java -Xmx1024M -Xms1024M -jar server.jar nogui
   ```

2. **Stopping the server**:
   ```bash
   stop
   ```

3. **Restarting the server**:
   - First, use the `stop` command and then execute the start command again.

### Server Settings:

1. **Editing server.properties**:
   ```bash
   nano /path/to/server/server.properties
   ```

2. **Editing the whitelist**:
   ```bash
   nano whitelist.json
   ```

3. **Editing Ops (Admins)**:
   ```bash
   nano ops.json
   ```

## 🎲 In-Game (Chat) Commands:

### General Commands:

1. **Help**:
   ```
   /help
   ```

2. **Set Game Mode**:
   ```
   /gamemode <mode> <player>
   ```

3. **Kick a Player**:
   ```
   /kick <player>
   ```

4. **Ban a Player**:
   ```
   /ban <player>
   ```

5. **Pardon (Unban) a Player**:
   ```
   /pardon <player>
   ```

6. **Whitelist a Player**:
   ```
   /whitelist add <player>
   ```

7. **Remove a Player from Whitelist**:
   ```
   /whitelist remove <player>
   ```

8. **Change Time**:
   ```
   /time set <value>
   ```

9. **Change Weather**:
   ```
   /weather <type>
   ```

10. **Teleport**:
   ```
   /tp <destination>
   ```

**Note**: Some commands may require admin privileges to execute.
```

---


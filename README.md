Vault Plugin
A powerful economy, chat, and permissions API for Minecraft servers.

📌 Features
✅ Supports multiple economy and permission plugins
✅ Provides a stable API for other plugins
✅ Easy integration with popular server plugins
✅ Efficient and lightweight

📥 Installation
Download the Vault JAR from here!
Place the JAR file into your server’s /plugins/ folder.
Restart your server to load Vault.
Configure Vault if necessary in config.yml.
⚙️ Configuration
Vault automatically integrates with supported economy and permission plugins.
To check if Vault is working correctly, use:

sh
Copy
Edit
/vault-info
This will display all connected plugins and their statuses.

🔌 Supported Plugins
Vault works with many economy, permission, and chat plugins, including:

EssentialsX
LuckPerms
PermissionsEx
CMI
Towny
And more!
📜 Commands
Command	Description
/vault-info	Shows Vault integration details
/vault-reload	Reloads Vault's configuration
📚 Developer API
Developers can hook into Vault to use economy, permissions, and chat features easily.
Example of adding Vault as a dependency in plugin.yml:

yaml
Copy
Edit
depend: [Vault]
Java API Example
java
Copy
Edit
RegisteredServiceProvider<Economy> rsp = getServer().getServicesManager().getRegistration(Economy.class);
Economy econ = rsp.getProvider();
double balance = econ.getBalance(player);
🛠 Troubleshooting
If Vault isn't working, make sure you have a compatible economy or permissions plugin installed.
Check for errors in the console (logs/latest.log).
Ensure your server is running a supported version of Paper, Spigot, or Bukkit.
📄 License
This project is open-source and licensed under the MIT License.

🔗 Useful Links
Official Wiki
Releases
Support

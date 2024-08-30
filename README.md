m-Logs System for FiveM
========================

Overview
--------
The m-Logs System is a FiveM script that logs player connections and disconnections to a Discord channel. It sends detailed information about each player, including their name, IP address (in spoiler format), Discord ID, Steam ID, ping, server ID, and licenses. This script is useful for server administrators to keep track of player activity.

Features
--------
- Logs player connections and disconnections.
- Sends detailed player information to Discord.
- Configurable webhooks for different events.
- Spoiler formatting for IP addresses to protect privacy.
- Easy to customize and extend.

Requirements
------------
- FiveM Server: Make sure your server is running on the latest version of FiveM.
- Discord Webhooks: You will need to set up webhooks in your Discord server to receive the logs.

Installation
------------
1. Download the Script:
   - Download the `m-logs.lua` file and place it in your server's resources directory.

2. Configure Webhooks:
   - Open the `m-logs.lua` file in a text editor.
   - Replace the placeholder webhook URLs (`PLACE_HERE_YOUR_WEBHOOK`) with your actual Discord webhook URLs.
   - You can use different webhooks for all events, player join, and player leave, or you can use the same webhook for all.

3. Add to Server Configuration:
   - Add the following line to your server’s `server.cfg` file to ensure the script is started with the server:
     ensure m-logs

4. Customize (Optional):
   - You can change the `name` and `logo` variables in the script to customize the appearance of the logs in Discord.

5. Restart Your Server:
   - Restart your FiveM server to apply the changes.

Usage
-----
Once installed and configured, the script will automatically start logging player connections and disconnections to the specified Discord webhooks. You don’t need to run any additional commands; everything is handled automatically.

Configuration Options
---------------------
- `webhookAll`: Webhook URL for sending logs of all events.
- `webhookJoin`: Webhook URL for sending logs of player joins.
- `webhookLeave`: Webhook URL for sending logs of player leaves.
- `name`: The username that will appear on the Discord messages.
- `logo`: The URL of the logo image that will appear on the Discord messages.

Support
-------
For any issues or customization requests, please contact the script creator or visit the FiveM forums for community support.

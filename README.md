# FiveM Discord Bot

A comprehensive Discord bot designed to interact with multiple FiveM servers. This bot provides various functionalities, including server uptime, player count, admin count, and more.

## Features

- Ping command to check bot latency
- List of libraries used by the bot
- Bot status and uptime
- FiveM server uptime
- Number of players online
- Number of admins online
- Paginated help command

## Installation

### Prerequisites

- [Node.js](https://nodejs.org/) (v14.0.0 or higher)
- [npm](https://www.npmjs.com/) (Node Package Manager)
- [Discord Account](https://discord.com/)
- [FiveM Server](https://fivem.net/)

### Steps

1. **Clone the repository:**

   ```sh
   git clone https://github.com/your-username/fivem-discord-bot.git
   cd fivem-discord-bot
Install dependencies:

sh
Copy code
npm install
Create a Discord bot:

Go to the Discord Developer Portal
Click on "New Application"
Navigate to the "Bot" tab and click "Add Bot"
Copy the bot token for later use
Configure the bot:

Rename data/servers.example.json to data/servers.json

Edit servers.json to include your server details:

json
Copy code
{
  "servers": [
    {
      "id": "server1",
      "name": "Example Server 1",
      "channelId": "YOUR_CHANNEL_ID_1",
      "ip": "SERVER_IP_1",
      "adminRoles": ["admin", "moderator"]
    },
    {
      "id": "server2",
      "name": "Example Server 2",
      "channelId": "YOUR_CHANNEL_ID_2",
      "ip": "SERVER_IP_2",
      "adminRoles": ["admin", "staff"]
    }
  ]
}
Set up environment variables:

Create a .env file in the root directory and add your bot token:

env
Copy code
DISCORD_TOKEN=YOUR_BOT_TOKEN
Start the bot:

sh
Copy code
npm start
Usage
Available Commands
!ping: Check the bot's latency.
!libraries: List the libraries used by the bot.
!status: Show the bot's status.
!uptime: Display the bot's uptime.
!downtime: Show the bot's last restart time.
!serveruptime <server_id>: Display the uptime of the specified FiveM server.
!players <server_id>: Show the number of players online on the specified FiveM server.
!admins <server_id>: Show the number of admins online on the specified FiveM server.
!help: Display a paginated help message with the list of commands.
Example Usage
Ping Command:

diff
Copy code
!ping
Response:

csharp
Copy code
Pong! Latency is 123ms. API Latency is 45ms.
Server Uptime:

diff
Copy code
!serveruptime server1
Response:

arduino
Copy code
Server uptime for Example Server 1 is: 3 hours, 25 minutes.
Players Count:

diff
Copy code
!players server1
Response:

arduino
Copy code
There are currently 15 players online on Example Server 1.
Admins Count:

diff
Copy code
!admins server1
Response:

arduino
Copy code
There are currently 3 admins online on Example Server 1.
Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
discord.js
FiveM
Node.js
markdown
Copy code

### Explanation

- **Introduction**: Provides an overview of the bot's purpose and features.
- **Installation**: Detailed steps on how to set up the bot, including cloning the repository, installing dependencies, creating a Discord bot, and configuring the bot.
- **Usage**: Describes the available commands and provides examples of how to use them.
- **Contributing**: Information on how to contribute to the project.
- **License**: License information.
- **Acknowledgements**: Credits to the libraries and tools used in the project.

This `README.md` should give users clear instructions on how to set up and use your FiveM Discord bot.

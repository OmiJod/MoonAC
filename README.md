Supported Inventory - 
QB / PS / LJ Inventory

Dependancy - ox_lib

Anticheat is now Released 
1 Month - https://moon-scriptsstore.tebex.io/package/6085872

3 Months - https://moon-scriptsstore.tebex.io/package/6085895

Life Time - https://moon-scriptsstore.tebex.io/package/6085897

Open Source - https://moon-scriptsstore.tebex.io/package/6085898

# Anti-Stacking Mechanism for Unique Items
1) Feature Description: Implements an automatic check to prevent players from stacking unique items in their inventory. If a unique item is found stacked (quantity more than one), the script unstacks it and sets the quantity back to one.

2) Player Notification: Logs detailed information, including the player's ID, name, Discord identifier, and action taken, whenever a unique item is unstacked.

3) Security Enhancement: This feature enhances server integrity by enforcing item uniqueness rules, preventing potential inventory exploits.
Automated Correction: Automatically adjusts the inventory without requiring manual intervention, ensuring a seamless experience for players and admins.
---------------------------------------------------
# Anti-Duplicate Weapon Serial Number System
1) Feature Description: This feature ensures the integrity of weapon ownership by preventing players from holding multiple weapons with the same serial number in their inventory. When a duplicate serial number is detected, the system automatically removes the extra weapons, leaving only one instance of the weapon with the unique serial number.

2) Implementation Details: The script iteratively checks each player's inventory for weapons. If it identifies weapons with the same serial number (indicating duplicates), it removes these duplicates, enforcing the rule that each weapon must have a unique serial number.

3) Player Notification & Logging: Whenever a duplicate weapon is removed, detailed information about the event is logged. This includes the player's Citizen ID, name, and details about the duplicate weapon. The logging system is designed to provide administrators with clear and actionable data for server management and player behavior monitoring.

4) Server Integrity: By preventing duplication of weapons, this feature upholds the server's gameplay balance and fairness. It deters potential exploits involving weapon duplication, contributing to a more stable and cheat-resistant gaming environment.
# -------------------------------------------------
# Cross-Table Duplicate Serial Number Check Command (/checkstashes)
1) Description: This command provides a robust solution for maintaining the integrity and uniqueness of weapon serial numbers across different storage systems in the game. When executed, it cross-checks weapon serial numbers among three key tables: stashitems, trunkitems, and gloveboxitems.

2) Functionality: On invocation, the command scans each table for weapon items and their associated serial numbers. It then identifies any serial number that appears in more than one table, signifying a duplicate across different storage locations.

3) Integrity Assurance: Ensures that each weapon in the game retains a unique serial number, crucial for tracking and ownership verification.
Exploit Prevention: Helps in preventing and identifying exploits related to weapon duplication, thereby maintaining fair gameplay.

4) Detailed Logging: Generates detailed logs for each duplicate found, including the type of storage, the specific item, and the conflicting serial number. This is essential for administrative oversight and resolving inventory discrepancies.
# Admin Command: openstash
1) Command Overview: The openstash command is a specialized tool designed for server administrators within the QBCore framework. It provides a powerful and direct way to access and manage different types of stashes (glovebox, stash) within the game.

2) Primary Use: This command is primarily used by administrators to efficiently address and resolve inventory-related issues, such as the removal of duplicate items from players' stashes. It streamlines the process of inventory management and oversight.

3) Command Syntax: /openstash [stashname]

stashname: The name of the stash to open. Valid options are 'glovebox', or 'stash'.
Functionality:

4) Direct Access: Allows admins to directly open specific stash types, providing immediate access to the contents without the need for navigating through the usual in-game interfaces.
Issue Resolution: Facilitates quick actions like identifying and removing duplicated items, thus maintaining the integrity and balance of the game economy.
Validation and Security: Incorporates checks to ensure that only valid stash names are accessed, preventing potential misuse or errors.
# ---------------------------------------------------
# Consolidated Logging for Duplicate Vehicle Deletion
1) Feature Description: Automates the detection and deletion of duplicate vehicles in-game. When duplicates are found, they are removed, and the action is logged.

2) Efficient Logging: Instead of individual logs for each deletion, the system generates a single consolidated log entry, detailing all deletions in one report for easier monitoring.

3) Enhanced Oversight: Improves server management by providing clear, concise logging of duplicate vehicle incidents, aiding in maintaining game integrity and reducing log clutter.
# --------------------------------------------------
# Negative Balance Monitoring and Logging
1) **Feature Description**: Monitors player balances for illegal negative amounts in cash, crypto, and bank accounts, aligning with server rules on permitted currency balances.

2) **Selective Logging**: Records instances of prohibited negative balances, logging only the affected currency types and relevant player details for efficient oversight.

3) **Server Integrity**: Enhances game fairness by ensuring economic rules are followed, providing a balanced gameplay environment.
# --------------------------------------------------
# AntiDuplicateLicense Monitoring and Enforcement

1) **Feature Description**: This feature actively scans and verifies player licenses within the server, aiming to prevent instances of duplicate licenses. It ensures each player has a unique identifier, maintaining the integrity of player identification and authentication.

2) **Selective Enforcement and Logging**: In cases where a duplicate license is detected, the feature logs detailed information about the involved parties. It records the license number along with relevant player information, such as Citizen ID and name. This selective approach focuses on specific incidents of license duplication, ensuring efficient tracking and management of these occurrences.

3) **Server Integrity and Fair Play**: By enforcing unique licenses for each player, the AntiDuplicateLicense feature upholds the server's standards for fair play and user authenticity. This contributes to a more secure and equitable gaming environment, where players can engage without concern over identity duplication or fraud.
# --------------------------------------------------
# ResetMoney Feature Overview

1) **Feature Description**: The `ResetMoney` feature offers administrative control over player finances within the game. It includes two key functions: resetting the money for all players and resetting the money for a specific player identified by their Citizen ID. This feature is designed to maintain economic balance and correct any discrepancies in player accounts.

2) **Selective and Total Reset Options**: Administrators have the flexibility to perform a selective reset for an individual player or a total reset affecting all players. The selective reset targets a specific player's financial data, ensuring targeted intervention without impacting other players. The total reset is used for broader financial adjustments, affecting all players equally.

3) **Server Integrity and Fair Play**: By providing tools to manage and correct player finances, the `ResetMoney` contributes significantly to the integrity and fairness of the game's economy. It helps to prevent and rectify financial exploits and anomalies, ensuring a balanced and equitable economic environment for all players.
# --------------------------------------------------
# Permissions - QBCore Permissions are used for this AntiCheat. You dont have to add any other thing except if you want to make more groups
#  --------------------------------------------------
# Anti-Pseudo Weapon Detection and Logging
1) **Feature Description**: This feature automates the detection of weapons that are added directly to a player's hand without being present in their inventory, a common exploit in cheats. When such a weapon is detected, it is removed from the player's possession, and the incident is logged for server administrators.

2) **Proactive Cheating Countermeasure**: This system serves as a proactive measure against common cheating techniques that bypass traditional inventory management. It ensures fair gameplay by enforcing the rule that all weapons must be legitimately obtained and stored in the player's inventory.

3) **Detailed Incident Reporting**: Each detection is accompanied by a detailed log entry, which includes the player's full name, server ID, and the specific weapon detected. This enhances server oversight by providing clear and actionable information about each incident, aiding in the identification of potential cheaters and maintaining the integrity of the game environment.
# ---------------------------------------------------
# Enhanced Anti-Cheat Resource Protection

**Feature Overview**: This robust feature enhances server security by monitoring and preventing unauthorized attempts to start or stop server resources. It's specifically designed to identify and counteract common cheating tactics that disrupt game integrity.

**Targeted Action**: When an illicit resource start/stop attempt is detected, the responsible player is immediately identified. The system differentiates between the offender and other players, ensuring precise and targeted enforcement actions: the offender is removed, while others are safely disconnected to maintain server stability.

**Automated Logging and Enforcement**: Each incident is automatically logged with detailed player information for administrative review. This streamlined process not only improves server management but also aids in swiftly addressing potential security breaches, ensuring a fair and cheat-free gaming environment.
# ---------------------------------------------------
# Advanced Anti-Blacklist Entity Monitoring
**Overview**: This feature actively monitors and controls the spawning of blacklisted entities, including vehicles, peds, and objects. It automatically identifies and addresses unauthorized entity creation in the game.

**Efficient Enforcement**: Upon detecting a blacklisted entity spawn, the entity is immediately despawned. The player responsible is identified, and appropriate actions are taken based on configurable settings: either kicking or removing the player.

**Real-Time Logging**: Each incident triggers a detailed log entry, specifying the entity details and the player involved. This assists in maintaining server integrity and provides a transparent audit trail for server administrators.
# ---------------------------------------------------
# Advanced Anti Weapon Damage Modifier

**Overview**: This feature detects and prevents the use of weapon damage modifiers in gameplay. It ensures fair play by identifying weapons with modified damage and taking action against the players using them.

**Automatic Detection**: The system constantly monitors weapon damage and compares it with the base damage. If a discrepancy is found, indicating a damage modifier, it either kicks or bans the player based on the server settings.

**Weapon Damage Table Command**: Administrators can easily generate a table of all weapon damages in the server with a simple command. This table can be added to the server's configuration to keep the anti-cheat system updated.

**Real-Time Logging**: Every incident of modified weapon damage is logged, providing server administrators with detailed information for review and action.
# ---------------------------------------------------
# Basic Anticheat Feature

1) **Actions**: Actions are only Taken When the Player is Completely Loaded and Logged into the server. In Short Players Wont be Bnned in Character Menu or Spawn Menu unlike other shit anticheats

2) **Features**: 
- Anti Noclip
- Anti Godmode
- Anti Invisible
- Anti Aim Assist
- Anti Infinite Stamina
- Anti God Health
- Anti God Armour
- Anti Resource Starter Stopper
- Anti Super Jump
- Anti Blacklist Keys
- Anti Explosive Bullets
- Anti Speed Hack
- Anti Blacklisted Weapons
- Anti High Ping
- Anti Spam Explosions
- Anti BlackList Name
- Anti Spam Peds
- Anti VPN
- Anti Spam Tazing  
- Anti BlackList Event Trigger



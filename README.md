# Skyrim Mod Data

## Contents

### mods.csv

Contains 5,000 records for mods collected from https://www.nexusmods.com/skyrim/mods/

- **Mod ID:** A unique identifier for the mod.
- **Name:** The name of the mod.
- **Category:** The category of the mod. The data contains 57 of the 61 mod categories for Skyrim, 1 of the 8 mod categories for Enderal (an overhaul mod that creates a completely new game using Skyrim as its base), and two mods that have no category listed.
  - Skyrim categories:
  - Enderal categories:
- **Endorsements:** The number of endorsements the mod has received. Endorsements are the equivalent of a _like_ or _thumbs up_. Only a user who has already downloaded the mod can endorse it.
- **Unique Downloads:** The number of different users who have downloaded the mod at least once.
- **Total Downloads:** The total number of times any user has downloaded the mod. This number is often significantly higher than unique downloads.
- **Views:** The number of times the mod has been viewed.
- **Last Update:** The date of the most recent update.
- **Original Upload:** The date the mod was originally uploaded to Nexus
- **Creator Name:** The name of the mod's creator, as provided by the uploader.
- **Uploader Name:** The uploader's user name. Often, but not always, the uploader is also the creator.
- **Uploader ID:** A unique identifier for the uploader.
- **Country:** The country the uploader is from (or claims to be from). Many users have not specified a country.
- **Date Collected:** The date the data was collected. Due to change over time, this is important to take note of.

### tags.csv

Contains 24,364 records, one for each tag attached to each of the 5,000 mods from mods.csv.

- **Mod ID:** A unique identifier for the mod.
- **Mod Name:** The name of the mod.
- **Tag:** The tag associated with the mod.
- **User ID:** A unique identifier for the uploader of the mod.
- **Country:** The country the uploader is from (or claims to be from). Many users have not specified a country.
- **Endorsements:** The number of endorsements the mod has received. Endorsements are the equivalent of a _like_ or _thumbs up_. Only a user who has already downloaded the mod can endorse it.
- **Unique Downloads:** The number of different users who have downloaded the mod at least once.
- **Total Downloads:** The total number of times any user has downloaded the mod. This number is often significantly higher than unique downloads.
- **Views:** The number of times the mod has been viewed.

## About the Data

Skyrim is a roleplaying video game featuring a fantasy setting and a huge world filled with locations to explore. Mods are special modifications that can be added to the game. Skyrim has a large "modding community" that creates and shares mods that do everything from overhauling the (somewhat abysmal) user interface (SkyUI) to turning all of the dragons into Thomas the Tank Engine characters (Really Useful Dragons). Players may have upwards of one or two hundred mods added to their game at any time.

All mods in this dataset were collected from Nexus, the primary site for hosting mods. They represent the top 5,000 (by number of endorsements) as of the time of collection. It is worth noting that not all of these are actually mods. For example, GEMS is a fancy list for Gameplay Enhancement Mods, and Forever Free is a logo that modders can use on their own mod pages.

There is a new edition of Skyrim - Skyrim Special Edition (SSE). Mods for this version are listed separately, and therefore are not included in this dataset. The data does, however, include a few mods for Enderal, a complete overhaul/new game using Skyrim as its base.

The data was scraped using Python (and Selenium). It was then cleaned to make it more useable in workshops and tutorials. For a list of changes made from the original scarped data, see below.

### Cleaning

#### Changes made to preserve original data

- fixed capitalization issues caused by web scraping
- removed leading and trailing whitespace
- merged a couple of tags with commas that got seperated

#### Changes made to the original data

- a few minor capitalization changes for consistency
- changed "- Other Languages" (tag) to "Other Languages"
- removed spaces between slashes for two tags (to match the other tags)
  - "Guilds / Factions" to "Guilds/Factions"
  - "Plants / Foliage" to "Plants/Foliage"
- edited country names
  - "Korea, Democratic People's Republic of" to "North Korea"
  - "Korea, Republic of" to "South Korea"
  - "Taiwan, Province of China" to "Taiwan"
- changed one instance (one mod, three tags) of user country from "none" to "Not Specified"

### Potential Issues

- Users can put whatever country they like.
- Data changes over time.
- There could be uncaught issues with the web scraping.

## Usage

Please feel free to use this dataset in your own workshops and tutorials.

Credit for gathering the data: Theo Acker, University of Oklahoma Libraries

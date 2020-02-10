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

- skyrim
- mods
- endorsements and downloads

## Collection

- collected from Nexus
- web scraping with Selenium (python)
- cleaned for easier usage

## Usage

## Issues

- users can put whatever country they like
- data changes over time
- could be uncaught issues with the web scraping




# seairdrop
Steem Engine Airdrop Tool
---

This tool will allow you to conduct your own airdrop without using any third party services.

## Supports all three distribution methods

* Transfer
* Issue
* Stake

## Requirements

* Python 3
* Beem Python Module

## Installation

Install Python 3

Install Requirements
`pip install -r requirements.txt`

## Usage

Create a text file with a list of all users and quantity of the token you want to distribute in a comma-separated file (CSV).

Any users that do not exist will be skipped automatically.

## Airdrop file

**airdrop.txt**:  

frank, 1000  
ned, 1000  
bob, 500  
ted, 200

Make a copy of config.json.example to config.json and edit the file.

In the configuration file you need to set the following information:

* account_name - Account you will distribute tokens from
* wif - Active key for this account (You can also use beem wallet)
* token - Name of the Steem Engine Token to airdrop
* memo - Memo to airdrop recipients
* mode - This can either be transfer, issue, stake
* delay - delay between users, recommended at least 10 seconds
* dry_run - True/False if you want to just do a test run

Once everything is set up, just need to do `python go.py <airdrop filename>` to start.

If you found this tool useful, send whatever you think this tool is worth to you in any token to @themarkymark.  

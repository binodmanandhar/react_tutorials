# React tutorials
Learning react

## Getting started

### HubSpot Theme – Local Development Setup

This repository contains a HubSpot CMS theme pulled locally using the **HubSpot CLI** and version-controlled with **GitHub**.

This guide explains how to set up the HubSpot CLI, authenticate your account, and pull the theme into your local environment.

---

### Prerequisites

Make sure the following are installed:

- **Node.js** (v16 or higher recommended)
- **npm** (comes with Node.js)
- **Git**
- A **HubSpot account** with CMS access

Check versions:
```bash
node -v
npm -v
git --version
```

----

### Install HubSpot CLI

Install the HubSpot CLI globally:
```sh
npm install -g @hubspot/cli
```
Verify installation:
```sh
hs version
```

### Authentication 
Documentation : [Source](https://developers.hubspot.com/docs/developer-tooling/local-development/hubspot-cli/reference)

Creates a config.yml file at the root of your home directory (i.e., ~/.hscli/config.yml), and sets up authentication for an account. 
If you’re adding authentication for a new account to an existing config file, run the auth command. When prompted for a name to use for the account, the name can’t contain spaces.

#### Based on global configuration for account management try below command

```
hs auth
```
OR
```
hs account auth
```


* Setup personal key
* Choose the HS portal
* After copy paste of personal key in the terminal, check whether we can access the account by using below command line.

```
hs accounts list
```
----

### Pulling theme into local directory

First pull the theme from git into local
```
git clone github_repository
```
* Then cd to the project folder
* The project folder should have README.md and theme_folder

#### Example to pull theme templates
```
hs cms fetch --account=<protal_id> hubspot_theme_name/templates theme_folder/templates
```

#### Example to pull individual module
```
hs cms fetch --account=<protal_id> hubspot_theme_name/modules/info-card.module theme_folder/modules/info-card.module 
```


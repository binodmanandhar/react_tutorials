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


* setup personal key
* After copy paste of personal key check whether the account is in the list by using below command

```
hs accounts list
```

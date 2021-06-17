# 🚀 GitHub Profile Views Counter
 
Many GitHub page views counters are not stable as it seems. Any service disruptions or simply removal of these services can lose your profile views. Use this GitHub Action to record changes. It generates badges, charts, and tables for each repository and a badge for total views for your profile. 

This action is written by [gayanvoice](https://github.com/gayanvoice). Don't forget to follow me on [GitHub](https://github.com/gayanvoice), [Medium](https://medium.com/@gayanvoice) and [Twitter](https://twitter.com/gayanvoice).

Before proceeding to set up this counter, look at this [repository](https://github.com/gayanvoice/insights). It uses this GitHub page views counter to record page views of each repository. You can select either `basic mode` or `advanced mode` to limit the information.

| Mode | Description |
| ---- | ----------- |
| `advanced` | `week` ✔️ `month` ✔️ `year` ✔️ |
| `basic` | `week` ✔️ `month` ❌ `year` ❌ |

## Setup

### Step 1 - ⚡️ Create an empty repository give it any name.

### Step 2 - 🔒 Generate a *personal access token* with `repo` and `workflow` options.
  
### Step 3 - 🔑 Create the *repository secret* name `INSIGHTS_TOKEN` and paste *personal access token* in value.

### Step 4 - 📄 Add list of repositories to `repository` in `config.json`.

### Step 5 - 🟥 Run actions.

## 📄 License
- Repository: [gayanvoice/github-profile-views-counter](https://github.com/gayanvoice/github-profile-views-counter)
- Source - [gayanvoice/github-insights](https://github.com/gayanvoice/github-insights)
- Code: [MIT](./LICENSE) © [Gayan Kuruppu](https://github.com/gayanvoice)

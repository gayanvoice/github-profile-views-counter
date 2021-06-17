# 🚀 GitHub Profile Views Counter
 
Many GitHub page views counters are not stable as it seems. Any service disruptions or simply removal of these services can lose your profile views. Use this GitHub Action to record changes. It generates badges, charts, and tables for each repository and a badge for total views for your profile. 

This action is written by [gayanvoice](https://github.com/gayanvoice). Don't forget to follow me on [GitHub](https://github.com/gayanvoice), [Medium](https://medium.com/@gayanvoice) and [Twitter](https://twitter.com/gayanvoice).

Before proceeding to set up this counter, look at this [repository](https://github.com/gayanvoice/insights). It uses this GitHub page views counter to record page views of each repository. You can select either `basic mode` or `advanced mode` to limit the information.

| Mode | Description |
| ---- | ----------- |
| `advanced` | `week` ✔️ `month` ✔️ `year` ✔️ |
| `basic` | `week` ✔️ `month` ❌ `year` ❌ |

## Setup

### Step 1 - ⚡️ Create an `empty repository` give it any name.

### Step 2 - 📄 Go to `Actions` create a `Simple workflow` by using `Set up this workflow` button.

### Step 3 - ✂️ Copy and 📋 paste the following script into the `yml` file.
```markdown
name: GitHub Profile Views Counter CI
on:
  schedule:
    - cron: '0 */6 * * *'
  workflow_dispatch:
jobs:
  release:
    name: GitHub Insights
    runs-on: ubuntu-20.04
    steps:
      - uses: actions/checkout@v2.3.4
        with:
          token: ${{ secrets.INSIGHTS_TOKEN }}
      - uses: actions/setup-node@v2.1.5
        with:
          node-version: 14.17.0
      - uses: gayanvoice/github-insights@1.0.0
        env:
          INSIGHTS_TOKEN: ${{ secrets.INSIGHTS_TOKEN }}
```
### Step 4 - 🔒 Generate a *personal access token* with `repo` and `workflow` options.
  
### Step 5 - 🔑 Create the *repository secret* name `INSIGHTS_TOKEN` and paste *personal access token* in value.

### Step 6 - 📄 Create a new file `config.json` and paste the following script.
```markdown
{
  "devMode": "false",
  "advancedMode": "true",
  "language": "en-US",
  "repository": [
    "android-vpn-client-ics-openvpn",
    "openvpn-install-for-multiple-users"
  ]
}
```
### Step 7 - 📄 Add list of repositories to `repository` in `config.json`.

### Step 8 - 🟥 Run actions.

## 📄 License
- Repository: [gayanvoice/github-profile-views-counter](https://github.com/gayanvoice/github-profile-views-counter)
- Source - [gayanvoice/github-insights](https://github.com/gayanvoice/github-insights)
- Code: [MIT](./LICENSE) © [Gayan Kuruppu](https://github.com/gayanvoice)

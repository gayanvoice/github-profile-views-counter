# 🚀 GitHub Profile Views Counter [<img alt="Image of my-profile-view-counter" src="https://github.com/gayanvoice/my-profile-view-counter/blob/master/graph/372372861/small/week.png" height="20">](https://github.com/gayanvoice/my-profile-view-counter/blob/master/readme/372372861/week.md)

[![Image of my-profile-view-counter](https://github.com/gayanvoice/my-profile-view-counter/blob/master/svg/372372861/badge.svg)](https://github.com/gayanvoice/my-profile-view-counter/blob/master/readme/372372861/week.md)

 
Many GitHub page views counters are not stable as it seems. Any service disruptions or simply removal of these services can lose your profile views. Use this GitHub Action to record changes. It generates badges, charts, and tables for each repository and a badge for total views for your profile.

## ▶️ Watch
[![How to Setup GitHub Profile Views Counter for your GitHub profile](https://img.youtube.com/vi/K6FYiP_XRuU/0.jpg)](https://www.youtube.com/watch?v=K6FYiP_XRuU)

## Why do you need 🚀 GitHub Profile Views Counter?
The main problem of using external services is what you do when they cut off their services? You will see a broken URL of the SVG you used to see profile views, and the next thing is you already lost thousands of profile views.

But this GitHub Profile Views Counter is different from others. It’s a public repository in your profile, and it stores all the data and SVG files. So you don’t lose anything, and it updates the page views every 6 hours. It fetches insights data of your repository from GitHub API. It records the number of unique visitors and also page views.

## Features
**Charts —** The action generates charts for the week, month, and year. The below chart is for the week for a repository. Go to gayanvoice/my-profile-view-counter to see how it works.

**Tables —** The action generates charts for the week, month, and year.
## Setup
**1 —** 🚀 Go to gayanvoice/github-profile-views-counter and click on **Use this template** button to create a new repository

By using a template you don’t need to create the files from scratch, and all you need is to change the configuration.

![GitHub Profile Views Counter - Click on Use this template button to create a new repository](https://miro.medium.com/max/600/1*wvbb87wOd1wCHKJh06vjPA.png)


**2 —** ⚡️ Enter a **repository name** and select repository type to **public repository** and click on **Create repository from template** button

You can give any name for the repository. You need to select repository type to public. Because GitHub provides an unlimited number of action minutes for public repositories.

If you choose private, the free usage will limit to 2000 minutes per month. Go to GitHub Pricing page for more pricing plans.

![GitHub Profile Views Counter - Click on create repository from template button to create the repository](https://miro.medium.com/max/600/1*hHdIM_fVnkdVdQGrbL1jRA.png)

After you click on **Create repository from template** button, it will take some time to create the repository.

**3 —** 🔒 Create a new personal access token with **repo** and **workflow** options

Go to Personal Access Tokens and click on Generate new token button. Give it any name and select repo and workflow options and click on Generate token button. ✂️ Copy the token.

![GitHub Profile Views Counter - create a new personal access token with repo and workflow options](https://miro.medium.com/max/700/1*YMft8U6IYTpBg7C5cASDUA.png)

**4 —** 🔑 Go to your profile views counter repository and go to **Settings**, and select **Secrets** option from left side bar. Click on **New repository secret** button and enter **name** as **INSIGHTS_TOKEN** and 📋 paste the **personal access token** under **value**. Click on **Add secret** button.

![GitHub Profile Views Counter - add repository secret by using repository secrets](https://miro.medium.com/max/700/1*jLtkxQNj2qrGcc4bLIvw3A.png)

**5 —** 📄 Go to your profile views counter repository. Go to **config.json** and click on edit button. Add repository names.

![GitHub Profile Views Counter - edit config.json file to add repository names](https://miro.medium.com/max/700/1*35wJBw75Fp5D_5t-fhaT_g.png)

**6 —** Go to your profile views counter repository and click on Actions tab. Select the workflow and click on **Run workflow** button.

![GitHub Profile Views Counter - click on run workflow button](https://miro.medium.com/max/700/1*hKkJ9EXlK14b3H3SeCNk4Q.png)

It will take few minutes depends on number of repositories you have entered to the workflow. It will generate total views badge, repository badges, and markdown files.

## 📄 License
- Repository: [gayanvoice/github-profile-views-counter](https://github.com/gayanvoice/github-profile-views-counter)
- Source - [gayanvoice/github-insights](https://github.com/gayanvoice/github-insights)
- Code: [MIT](./LICENSE) © [Gayan Kuruppu](https://github.com/gayanvoice)

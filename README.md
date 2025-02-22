# GitHub Action Reusable Workflows

## :exclamation: Keep up-to-date with GitHub Dependabot


| :warning: UPDATE    |
|:--------------------|
| The following is not yet available as part of Dependabots package ecosystem.<br/>https://github.community/t/dependabot-with-reusable-workflow-versions/207372/4 |


Since [Dependabot](https://docs.github.com/en/github/administering-a-repository/keeping-your-actions-up-to-date-with-github-dependabot) has [native GitHub Actions support](https://docs.github.com/en/github/administering-a-repository/configuration-options-for-dependency-updates#package-ecosystem), to enable it on your GitHub repo all you need to do is add the `.github/dependabot.yml` file:

```yml
version: 2
updates:
  # Maintain dependencies for GitHub Actions
  - package-ecosystem: "github-actions"
    directory: "/"
    schedule:
      interval: "daily"
```
gh actions-importer version$ gh actions-importer version
gh version 2.14.3 (2022-07-26)
gh actions-importer        github/gh-actions-importer v0.1.12
actions-importer/cli       unknowngh extension install github/gh-actions-importer$ gh extension install github/gh-actions-importer
✓ Installed extension github/gh-actions-importer/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)https://raw.githubusercontent.com/Homebrew/install/HEAD/install.shconda install ghmamba install ghpost-link.shpre-unlink.batpre-link.shconda search gh --channel conda-forge# Travis CI migrations powered by GitHub Actions Importer

The instructions below will guide you through configuring a GitHub Codespaces environment that your will use in subsequent labs to learn how to use GitHub Actions Importer to migrate Travis CI pipelines to GitHub Actions.

These steps **must** be completed prior to starting other labs.

## Create your own repository for these labs

1. Ensure that you have created a repository using the [actions/importer-labs](https://github.com/actions/importer-labs) as a template.

## Configure your codespace

1. Start a new codespace.

    - Click the `Code` button on your repository's landing page.
    - Click the `Codespaces` tab.
    - Click `Create codespaces on main` to create the codespace.
    - After the Codespace has initialized there will be a terminal present.

2. Verify the GitHub Actions Importer CLI is installed and working. More information on the GitHub Actions Importer extension for the official GitHub CLI can be found [here](https://github.com/github/gh-actions-importer).

    - Run the following command in the codespace terminal:

      ```bash
      gh actions-importer version
      ```

    - Verify the output is similar to below.

      ```console
      $ gh actions-importer version
      gh version 2.14.3 (2022-07-26)
      gh actions-importer        github/gh-actions-importer v0.1.12
      actions-importer/cli       unknown
      ```

    - If `gh actions-importer version` did not produce similar output, please refer to the [troubleshooting section](#troubleshoot-the-github-actions-importer-cli).

## Labs for Travis CI

Perform the following labs to learn more about how to migrate Travis CI pipelines to GitHub Actions using GitHub Actions Importer:

1. [Configure credentials for GitHub Actions Importer](1-configure.md)
2. [Perform an audit of Travis CI](2-audit.md)
3. [Forecast potential build runner usage](3-forecast.md)
4. [Perform a dry-run of a Travis CI pipeline](4-dry-run.md)
5. [Use custom transformers to customize GitHub Actions Importer's behavior](5-custom-transformers.md)
6. [Perform a production migration of a Travis CI pipeline](6-migrate.md)

## Troubleshoot the GitHub Actions Importer CLI

The CLI extension for GitHub Actions Importer can be manually installed by following these steps:

- Verify you are in the codespace terminal
- Run this command from within the codespace's terminal:

  ```bash
  gh extension install github/gh-actions-importer
  ```

- Verify the result of the install contains:

  ```console
  $ gh extension install github/gh-actions-importer
  ✓ Installed extension github/gh-actions-importer
  ```

- Verify GitHub Actions Importer CLI extension is installed and working by running the following command from the codespace terminal:

  ```bash
  gh actions-importer version
  ```
    Welcome to Apache's Jira issue tracker!

Anyone is free to find issues. You must register and login if you want to create, comment or vote on, or watch issues. Only developers can edit, prioritize, schedule or resolve issues.

Note that public signup for this Jira instance is disabled. Go to the self-serve signup page to apply for an account, which needs a projects approval.

We migrated some projects here from Bugzilla. If you had a Bugzilla account, log in using your email address as your username. You will need to have a new password mailed to you. You can search for issues by their old Bugzilla IDs in the quick search box above.

Need to create an INFRA ticket? See the INFRA Jira Guidelines on the Infra Website.

If your ASF project wants to use Jira goto our selfserve to setup a new project.

PRIVACY NOTICE: ASF Jira is an open issue tracking system. Activity on most issues, will be publicly visible. Email addresses are not visible to other users unless you set your email address as your username
	![Icosahedral_tensegrity_structure.png](https://github.com/yangsenius/learning-to-learn-by-pytorch/assets/88852908/c1c43654-15d8-483c-b96b-adb18e271284)
https://travis-ci.comer version
gh version 2.14.3 (2022-07-26)
gh actions-importer        github/gh-actions-importer v0.1.12
actions-importer/cli       unknownhttps://github.com$ gh actions-importer configure
✔ Which CI providers are you configuring?: Travis CI
Enter the following values (leave empty to omit):
✔ Personal access token for GitHub: ***************
✔ Base url of the GitHub instance: https://github.com
✔ Personal access token for Travis CI: ***************
✔ Base url of the Travis CI instance: https://travis-ci.com
✔ Travis CI organization name: actions-importer-labs
Environment variables successfully updated.

<div align="center">
    <picture>
        <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/7659/174594540-5e29e523-396a-465b-9a6e-6cab5b15a568.svg">
        <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/7659/174594559-0b3ddaa7-e75b-4f10-9dee-b51431a9fd4c.svg">
        <img src="https://user-images.githubusercontent.com/7659/174594540-5e29e523-396a-465b-9a6e-6cab5b15a568.svg" alt="Dependabot" width="336">
    </picture>
</div>

## Dependabot Demo Repository

This repo contains some projects with outdated dependencies. Fork it to try out
Dependabot :dependabot:!

### Enabling Security Updates

- In your fork, click the **Settings** tab
- In the left hand side navigation, click **Code security and analysis**
- Enable **Dependabot security updates** or **Grouped security updates**
- Dependabot will now start creating PRs for detected security vulnerabilities
- Go into the **Security** tab and click **Dependabot** in the left hand side navigation to see what Dependabot is working on

<img width="929" alt="screenshot showing Dependabot working on Security Updates" src="https://github.com/dependabot/demo/assets/886768/9295c61a-631b-4c56-9c00-ff078874f362">

After about 5 minutes you should see some PRs open. Merge them and the Securty Alerts will close 🎉

### Enabling Version Updates

This demo includes a `dependabot.yml` which configures [Version Updates](https://docs.github.com/github/administering-a-repository/keeping-your-dependencies-updated-automatically), but forks don't automatically start with Dependabot enabled.

The enable Dependabot on your fork:
- Click the **Insights** tab
- In the left hand side navigation, click **Dependency Graph**
- Click on the **Dependabot** tab
- Click on the **Enable Dependabot** button

Running commit update to trigger Dependabot Review Workflow
- After a moment, refresh the page and you should see Dependabot hard at work

<img width="917" alt="screenshot showing Dependabot working on Version Updates" src="https://github.com/dependabot/demo/assets/886768/4adf5727-255a-4ae1-97f7-70e94dc1134b">

After a few minutes, you should get some more PRs!

### Security updates are vulnerability-driven; version updates are freshness-driven.

Dependabot security updates open PRs when GitHub detects a known vulnerable dependency in your project and a safer version is available.
Dependabot version updates open PRs to keep dependencies up to date more generally, even when there’s no known security issue.
In this repo’s README:

Under Enabling Security Updates, it says Dependabot will create PRs for detected security vulnerabilities.
Under Enabling Version Updates, it references the dependabot.yml config, which controls routine dependency update behavior.
Practical difference:

### Why the PR is created

Security update: fix a known CVE/advisory.
Version update: move to newer dependency versions proactively.
What triggers it

Security update: vulnerability detection from GitHub’s security alerts.
Version update: the dependabot.yml schedule/config and available newer releases.
Goal

Security update: reduce immediate security risk.
Version update: reduce staleness, keep compatibility current, and avoid big upgrade jumps later.
Urgency

Security updates are usually higher priority.
Version updates are usually maintenance wor

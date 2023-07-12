# Automated dependency updates

[Renovate][1] applied to all current and future projects in the arcalot GitHub org

## Voting Period

The voting period for this proposal will be open for 10 days from its submission.

## Benefits

Renovate is a tool that automates dependency updates in your repository by opening pull requests for you. Here are some of the benefits of using Renovate:

1. Save time and effort: Manually updating dependencies can be time-consuming and error-prone, especially if you have many repositories to maintain. Renovate automates the process by automatically checking for updates and opening pull requests, saving you time and effort.

2. Keep dependencies up-to-date: Keeping dependencies up-to-date is important to ensure that your code is secure, reliable, and compatible with the latest technologies. Renovate helps you stay up-to-date by regularly checking for updates and opening pull requests to update dependencies.

3. Reduce security risks: Outdated dependencies can pose security risks, as they may contain known vulnerabilities that can be exploited by attackers. Renovate helps you reduce security risks by automatically updating your dependencies to their latest secure versions.

4. Improve stability and performance: Updating dependencies can improve the stability and performance of your code. Renovate helps you stay up-to-date with the latest versions of your dependencies, which can help you identify and fix bugs, and improve the performance of your code.

5. Customizable configurations: Renovate offers customizable configurations that allow you to tailor the tool to your specific needs. You can customize update schedules, branch names, and other settings to fit your workflow.

Overall, Renovate can help you save time and effort, improve the security, stability, and performance of your code, and customize the tool to fit your specific needs.

## Renovate vs. Dependabot

Both Renovate and Dependabot are excellent tools for automating dependency updates in your repositories. Here are some reasons why you might choose Renovate over Dependabot:

1. More flexible configuration: Renovate offers more flexible configuration options than Dependabot, allowing you to fine-tune the update behavior to match your needs. Renovate's configuration options include things like update schedules, filtering rules, and package manager-specific options.

2. Better update handling: Renovate can handle complex updates better than Dependabot, which is especially useful when you have dependencies with multiple release channels or non-standard versioning schemes.

3. More supported package managers: Renovate supports a wider range of package managers than Dependabot, including Yarn, Pip, and Rubygems.

4. More frequent updates: Renovate has a more frequent update schedule than Dependabot, which means you can get updates to the tool and its dependencies faster.

5. Stronger community support: Renovate has a strong and active community of users and contributors who can provide support and contribute to the tool's development.

That being said, Dependabot is still a great tool for automating dependency updates, and may be a better fit for your specific needs. Ultimately, the choice between Renovate and Dependabot depends on your specific use case and preferences.

## Drawbacks

While Renovate can be a powerful tool for automating dependency updates, there are a few potential drawbacks to consider:

1. Pull request overload: Renovate can generate a large number of pull requests, especially if you have many repositories or dependencies. This can create a lot of noise in your pull request feed and may require additional effort to manage.

2. False positives: Renovate may sometimes generate pull requests for updates that don't actually improve your dependencies or may introduce new issues. This can create additional work and may require manual intervention to resolve.

3. Configurability complexity: While Renovate offers a lot of configuration options, this can also make it more complex to set up and manage than other dependency update tools.

4. Limited control over updates: Renovate automates the update process, but you may not have full control over which updates are applied to your dependencies. This can be a concern if you need to ensure strict compatibility or stability with certain packages or versions.

5. Potential conflicts with other automation: If you have other automation tools or processes in place that also manage dependency updates, Renovate may conflict with them and create additional work or confusion.

6. Renvoate GitHub app installation requires creating an account, sharing personal data and granting permissions to a third party.

Overall, the benefits of using Renovate may outweigh these potential drawbacks, but it's important to consider these factors and weigh them against your specific use case and needs.

## Roll Out

- A self-hosted renovate [repo][2]
- As soon as the workflow is activated on the repositories (all or one by one), renovate generates a PR with a basic configuration file [Example repo][3]
- Additional customizations might be applied
- Disabling Dependabot

[1]: https://docs.renovatebot.com/
[2]: https://github.com/platform-engineering-org/self-hosted-renovate
[3]: https://github.com/platform-engineering-org/arcaflow-engine

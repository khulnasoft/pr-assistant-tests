# Overview

KhulnaSoft PR-Assistant is an open-source tool to help efficiently review and handle pull requests.

- See the [Installation Guide](./installation/index.md) for instructions on installing and running the tool on different git platforms.

- See the [Usage Guide](./usage-guide/index.md) for instructions on running the PR-Assistant commands via different interfaces, including _CLI_, _online usage_, or by _automatically triggering_ them when a new PR is opened.

- See the [Tools Guide](./tools/index.md) for a detailed description of the different tools.


## PR-Assistant Features
PR-Assistant offers extensive pull request functionalities across various git providers.

|       |                                                                                                                       | GitHub | Gitlab | Bitbucket | Azure DevOps |
|-------|-----------------------------------------------------------------------------------------------------------------------|:------:|:------:|:---------:|:------------:|
| TOOLS | Review                                                                                                                |   ✅    |   ✅    |   ✅       |      ✅      |
|       | ⮑ Incremental                                                                                                         |   ✅    |        |            |              |
|       | ⮑ [SOC2 Compliance](https://khulnasoft.github.io/tools/review/#soc2-ticket-compliance){:target="_blank"} 💎        |   ✅    |   ✅    |   ✅        |      ✅      |
|       | Ask                                                                                                                   |   ✅    |   ✅    |   ✅        |      ✅      |
|       | Describe                                                                                                              |   ✅    |   ✅    |   ✅        |      ✅      |
|       | ⮑ [Inline file summary](https://khulnasoft.github.io/tools/describe/#inline-file-summary){:target="_blank"} 💎     |   ✅    |   ✅    |           |      ✅      |
|       | Improve                                                                                                               |   ✅    |   ✅    |   ✅        |      ✅      |
|       | ⮑ Extended                                                                                                            |   ✅    |   ✅    |   ✅        |      ✅      |
|       | [Custom Prompt](./tools/custom_prompt.md){:target="_blank"} 💎                                                        |   ✅    |   ✅    |   ✅        |      ✅      |
|       | Reflect and Review                                                                                                    |   ✅    |   ✅    |   ✅        |      ✅      |
|       | Update CHANGELOG.md                                                                                                   |   ✅    |   ✅    |   ✅        |      ️       |
|       | Find Similar Issue                                                                                                    |   ✅    |        |             |      ️       |
|       | [Add PR Documentation](./tools/documentation.md){:target="_blank"} 💎                                                 |   ✅    |   ✅    |          |      ✅      |
|       | [Generate Custom Labels](./tools/describe.md#handle-custom-labels-from-the-repos-labels-page-💎){:target="_blank"} 💎 |   ✅    |   ✅    |            |      ✅      |
|       | [Analyze PR Components](./tools/analyze.md){:target="_blank"} 💎                                                      |   ✅    |   ✅    |       |      ✅      |
|       |                                                                                                                       |        |        |            |      ️       |
| USAGE | CLI                                                                                                                   |   ✅    |   ✅    |   ✅       |      ✅      |
|       | App / webhook                                                                                                         |   ✅    |   ✅    |    ✅        |      ✅      |
|       | Actions                                                                                                               |   ✅    |        |            |      ️       |
|       |                                                                                                                       |        |        |            |
| CORE  | PR compression                                                                                                        |   ✅    |   ✅    |   ✅       |   ✅        |
|       | Repo language prioritization                                                                                          |   ✅    |   ✅    |   ✅       |   ✅        |
|       | Adaptive and token-aware file patch fitting                                                                           |   ✅    |   ✅    |   ✅     |   ✅        |
|       | Multiple models support                                                                                               |   ✅    |   ✅    |   ✅       |   ✅        |
|       | Incremental PR review                                                                                                 |   ✅    |        |            |           |
|       | [Static code analysis](./tools/analyze.md/){:target="_blank"} 💎                                                      |   ✅    |   ✅     |    ✅    |   ✅        |
|       | [Multiple configuration options](./usage-guide/configuration_options.md){:target="_blank"} 💎                         |   ✅    |   ✅     |    ✅    |   ✅        |

💎 marks a feature available only in [PR-Assistant Pro](https://www.khulnasoft.com/pricing/){:target="_blank"}


## Example Results
<hr>

#### [/describe](https://github.com/khulnasoft/pr-assistant/pull/530)
<figure markdown="1">
![/describe](https://www.khulnasoft.com/images/pr_assistant/describe_new_short_main.png){width=512}
</figure>
<hr>

#### [/review](https://github.com/khulnasoft/pr-assistant/pull/732#issuecomment-1975099151)
<figure markdown="1">
![/review](https://www.khulnasoft.com/images/pr_assistant/review_new_short_main.png){width=512}
</figure>
<hr>

#### [/improve](https://github.com/khulnasoft/pr-assistant/pull/732#issuecomment-1975099159)
<figure markdown="1">
![/improve](https://www.khulnasoft.com/images/pr_assistant/improve_new_short_main.png){width=512}
</figure>
<hr>

#### [/generate_labels](https://github.com/khulnasoft/pr-assistant/pull/530)
<figure markdown="1">
![/generate_labels](https://www.khulnasoft.com/images/pr_assistant/geneare_custom_labels_main_short.png){width=300}
</figure>
<hr>

## How it Works

The following diagram illustrates PR-Assistant tools and their flow:

![PR-Assistant Tools](https://khulnasoft.com/images/pr_assistant/diagram-v0.9.png)

Check out the [PR Compression strategy](core-abilities/index.md) page for more details on how we convert a code diff to a manageable LLM prompt



## PR-Assistant Pro 💎

[PR-Assistant Pro](https://www.khulnasoft.com/pricing/) is a hosted version of PR-Assistant, provided by KhulnaSoft. It is available for a monthly fee, and provides the following benefits:

1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Assistant app to your GitHub\GitLab\BitBucket repo.
2. **Improved privacy** - No data will be stored or used to train models. PR-Assistant Pro will employ zero data retention, and will use an OpenAI account with zero data retention.
3. **Improved support** - PR-Assistant Pro users will receive priority support, and will be able to request new features and capabilities.
4. **Extra features** -In addition to the benefits listed above, PR-Assistant Pro will emphasize more customization, and the usage of static code analysis, in addition to LLM logic, to improve results. It has the following additional tools and features:
    - (Tool): [**Analyze PR components**](./tools/analyze.md/)
    - (Tool): [**Custom Prompt Suggestions**](./tools/custom_prompt.md/)
    - (Tool): [**Tests**](./tools/test.md/)
    - (Tool): [**PR documentation**](./tools/documentation.md/)
    - (Tool): [**Improve Component**](https://khulnasoft.github.io/tools/improve_component/)
    - (Tool): [**Similar code search**](https://khulnasoft.github.io/tools/similar_code/)
    - (Tool): [**CI feedback**](./tools/ci_feedback.md/)
    - (Feature): [**Interactive triggering**](./usage-guide/automations_and_usage.md/#interactive-triggering)
    - (Feature): [**SOC2 compliance check**](./tools/review.md/#soc2-ticket-compliance)
    - (Feature): [**Custom labels**](./tools/describe.md/#handle-custom-labels-from-the-repos-labels-page)
    - (Feature): [**Global and wiki configuration**](./usage-guide/configuration_options.md/#wiki-configuration-file)
    - (Feature): [**Inline file summary**](https://khulnasoft.github.io/tools/describe/#inline-file-summary)

   
## Data Privacy

### Self-hosted PR-Assistant

- If you host PR-Assistant with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
https://openai.com/enterprise-privacy

### KhulnaSoft-hosted PR-Assistant Pro 💎

- When using PR-Assistant Pro 💎, hosted by KhulnaSoft, we will not store any of your data, nor will we use it for training. You will also benefit from an OpenAI account with zero data retention.

- For certain clients, KhulnaSoft-hosted PR-Assistant Pro will use KhulnaSoft’s proprietary models — if this is the case, you will be notified.

- No passive collection of Code and Pull Requests’ data — PR-Assistant will be active only when you invoke it, and it will then extract and analyze only data relevant to the executed command and queried pull request.

### PR-Assistant Chrome extension

- The [PR-Assistant Chrome extension](https://chromewebstore.google.com/detail/pr-assistant-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) serves solely to modify the visual appearance of a GitHub PR screen. It does not transmit any user's repo or pull request code. Code is only sent for processing when a user submits a GitHub comment that activates a PR-Assistant tool, in accordance with the standard privacy policy of PR-Assistant.
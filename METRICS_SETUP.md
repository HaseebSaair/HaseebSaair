# Publish and Metrics setup

## 1. Create the profile repository

Create a **public** GitHub repository named exactly `HaseebSaair`. GitHub displays the repository's `README.md` on your profile because its name matches your username.

## 2. Add these files

- Put `README.md` in the repository root.
- Put `metrics.yml` at `.github/workflows/metrics.yml`.
- Confirm the LinkedIn and email links in `README.md` open correctly.

## 3. Prepare Starred Topics

The Starred Topics graphic is not a tech-stack card. It shows topics you genuinely follow.

1. Visit <https://github.com/topics>.
2. Star only topics that reflect your real interests.
3. A focused starting set could include `artificial-intelligence`, `machine-learning`, `large-language-models`, `ai-agents`, `automation`, `n8n`, `geospatial`, and `cloud-computing`.

Keep the list intentional. The workflow displays at most 12 topics.

## 4. Create the Metrics secret

The half-year isometric calendar needs a GitHub personal access token.

1. In GitHub, open **Settings → Developer settings → Personal access tokens**.
2. Create a classic token named `metrics-profile` with no scopes for public-only metrics. Use the least privilege possible.
3. Open the `HaseebSaair` repository, then go to **Settings → Secrets and variables → Actions**.
4. Create a repository secret named `METRICS_TOKEN` and paste the token as its value.

Never paste the token into `README.md` or `metrics.yml`.

## 5. Generate the graphics

1. Open the repository's **Actions** tab.
2. Select **Profile metrics**.
3. Choose **Run workflow**.
4. When it finishes, confirm that these files exist in the repository root:
   - `metrics.plugin.topics.svg`
   - `metrics.plugin.isocalendar.svg`

The workflow refreshes them daily and can also be run manually.

## 6. Final profile checks

- Pin `punjab-smokewatch` and `invoice-automation-n8n` on the GitHub profile.
- Add concise descriptions and relevant topics to both repositories.
- Confirm the LinkedIn link, email link, project links, and live demo all open correctly.
- Preview the profile on both desktop and mobile before sharing it.

Official references: [Metrics setup](https://github.com/lowlighter/metrics#%EF%B8%8F-using-github-action-on-a-profile-repository-10-min), [Isometric Calendar](https://github.com/lowlighter/metrics/blob/master/source/plugins/isocalendar/README.md), and [Starred Topics](https://github.com/lowlighter/metrics/blob/master/source/plugins/topics/README.md).

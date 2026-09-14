# BLADE_Alpha — bright-garden test environment

Preview GitHub Pages site for the `bright-garden` branch of [`dad2lna-coder/BLADE_Alpha`](https://github.com/dad2lna-coder/BLADE_Alpha/tree/bright-garden).

## Live preview

**https://dad2lna-coder.github.io/BLADE_Alpha-bright-garden/**

Production (`main`) stays at **https://dad2lna-coder.github.io/BLADE_Alpha/**

## How this works

This repo does not hold the app source. On every push to `main` here, on manual *Run workflow*, and on a 6-hour schedule, Actions:

1. Checks out `dad2lna-coder/BLADE_Alpha` @ `bright-garden`
2. Copies the static web app (`index.html`, `css/`, `js/`, `lib/`, `modules/`, `airport/`)
3. Deploys it to this repo's GitHub Pages site

## Refresh after source changes

After you push to `bright-garden`:

1. Open [Actions → Deploy bright-garden Pages](https://github.com/dad2lna-coder/BLADE_Alpha-bright-garden/actions/workflows/deploy-pages.yml)
2. Click **Run workflow**

Or wait for the scheduled refresh.

## First-time Pages note

If the first deploy fails with a Pages environment error, open
**Settings → Pages** on this repo and set Source to **GitHub Actions**, then re-run the workflow.

# Yitavo public site

Source for Yitavo's public homepage and privacy policy, the two pages Google's OAuth consent screen requires. They are meant to be served free by GitHub Pages at `https://yitavo.github.io`, with the privacy policy at `https://yitavo.github.io/privacy/`.

`github.io` is on the Public Suffix List, so `yitavo.github.io` counts as its own top private domain that only the `yitavo` GitHub organization controls. Google's docs don't name github.io, so its acceptance for brand verification is inferred, not yet proven.

## Publish

1. Create the free GitHub organization `yitavo` (github.com/account/organizations/new, Free plan).
2. In it, create a public repository named exactly `yitavo.github.io` and copy these files to its root, keeping `.nojekyll`. Pages publishes an organization's `<org>.github.io` repository from its default branch.
3. Check both URLs load while signed out.

## Google steps

1. Search Console: add `https://yitavo.github.io/` as a URL-prefix property and verify it with the HTML file method (add the file Google gives you next to `index.html`).
2. Google Cloud, with a standard project (Apps Script: Project Settings, change the Cloud project): on the branding page set app name Yitavo, homepage `https://yitavo.github.io`, privacy policy `https://yitavo.github.io/privacy/`, authorized domain `yitavo.github.io`.
3. Before submitting brand verification, make sure the privacy policy lists what each Apps Script tool actually requests. Update the "Google data we use" section if a tool needs more than sign-in, `drive.file`, or data it processes in the user's own account.

## Before relying on it

- Replace the GitHub-issues contact with a private contact address when one exists.
- The legal entity is still pending (founder decision F6). Add it to the footer and policy once it exists.

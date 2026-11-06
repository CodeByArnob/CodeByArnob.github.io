# FoodLens Account Connection Portal

This repository hosts the official GitHub Pages origin reserved for FoodLens account connection.

Website: https://codebyarnob.github.io/

## Security status

The current page is a static status/landing page only. It does not authenticate users, collect credentials, receive Puter tokens, or claim that a browser session has been transferred to the Android app.

The native authentication flow must not be enabled until a provider-supported authorization handoff is confirmed and validated. In particular:

- Never place Puter tokens or authorization codes in ordinary URL query parameters.
- Never scrape Chrome cookies or browser storage.
- Never embed developer secrets in this public repository.
- Validate callback state, origin, transaction lifetime, and one-time use.
- Verify the resulting Puter identity and AI access before marking FoodLens connected.

## GitHub Pages

The site is intended to deploy from GitHub Actions using the Pages deployment workflow in `.github/workflows/pages.yml`.

After the first workflow is committed, verify that Pages is enabled in repository Settings → Pages and that the source is set to GitHub Actions.

## Related project

- [FoodLens Android application](https://github.com/CodeByArnob/FoodLens)
- [Authentication investigation](https://github.com/CodeByArnob/FoodLens/issues/1)

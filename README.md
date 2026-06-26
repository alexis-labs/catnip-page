# Catnip Money Privacy Policy Website

This repository contains a static, GitHub Pages-ready privacy policy website for the Android game **Catnip Money**.

## Files

- `index.html` - the full Privacy Policy page and Google Play Data Safety Mapping section.
- `styles.css` - responsive, accessible styling.
- `README.md` - deployment and editing instructions.

## Before publishing

Replace these placeholders and review the policy against the real app build:

- `[Developer / Company Name]` in `index.html`
- `privacy@catnipmoney.app` if you use a different contact email
- `https://catnipmoney.app/` in the canonical and Open Graph URL tags
- Third-party service references if your app does not use Supabase, CoinGecko, or any other listed provider
- The effective date and last updated date when the policy changes

If you add ads, analytics, crash reporting, purchases, sign-in, cloud saves, push notifications, or any other SDK, update both this policy and the Google Play Data safety form.

## Deploy to GitHub Pages

1. Push this repository to GitHub.
2. Open the repository on GitHub.
3. Go to **Settings** > **Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the branch you want to publish, usually `main`.
6. Select the root folder, `/`.
7. Click **Save**.

GitHub will publish the site at a URL like:

```text
https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/
```

After GitHub Pages finishes deploying, open the URL and verify that the policy page loads on desktop and mobile.

## How to edit the policy text

Edit `index.html` directly. Each policy topic is in its own `<section>` with an `id`, such as:

```html
<section id="data-we-collect">
```

Keep the section headings and wording aligned with the actual game behavior. Do not list services, SDKs, or data uses that the app does not actually have.

When you update the policy:

1. Update the **Last updated** date near the top of `index.html`.
2. Update any changed data collection, sharing, retention, or deletion details.
3. Re-check the **Data Safety Mapping** table at the bottom.
4. Re-deploy through GitHub Pages.

## How to set a custom domain later

1. Buy or configure a domain, for example `catnipmoney.app`.
2. In GitHub, go to **Settings** > **Pages**.
3. Enter your custom domain in the **Custom domain** field.
4. Save the setting.
5. In your domain DNS provider, add the DNS records GitHub Pages requires.
6. After DNS resolves, enable **Enforce HTTPS** in GitHub Pages.
7. Update `index.html` so the canonical URL and Open Graph URL use the custom domain:

```html
<link rel="canonical" href="https://catnipmoney.app/">
<meta property="og:url" content="https://catnipmoney.app/">
```

## Where to use the final URL in Google Play Console

After the site is live, paste the published privacy policy URL in:

**Google Play Console** > **App content** > **Privacy Policy**

Also use the policy and the **Data Safety Mapping** section as a reference when completing:

**Google Play Console** > **App content** > **Data safety**

The Data safety answers must match the actual app build and SDKs, not only this website text.

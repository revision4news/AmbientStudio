# Ambient Studio: website, Privacy Policy and Terms

The public pages the TikTok, Meta and Google developer apps ask for. Plain HTML, ready for GitHub Pages.

| File | Page |
|---|---|
| `index.html` | Home: what Ambient Studio is |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms of Service |
| `data-deletion.html` | Data deletion instructions |

## Publish on GitHub Pages

Push **only this folder**. Never push the rest of `ambient-studio`: `config.yaml` and `client_secret.json` hold your secrets.

1. On GitHub, create a new **public** repository, for example `ambient-studio-site`.
   Naming it `<your-username>.github.io` instead serves the pages at the root of that address.
2. Push this folder to it:

   ```bash
   cd ~/workplace/ambient-studio/legal-site
   git init
   git add .
   git commit -m "Ambient Studio website, privacy policy and terms"
   git branch -M main
   git remote add origin https://github.com/<your-username>/ambient-studio-site.git
   git push -u origin main
   ```

   Or use **Add file → Upload files** on the new repository and drop these files in.
3. In the repository: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`, **Save**. The site is live a minute or two later.

The pages are then at:

- Home: `https://<your-username>.github.io/ambient-studio-site/`
- Privacy Policy: `https://<your-username>.github.io/ambient-studio-site/privacy.html`
- Terms of Service: `https://<your-username>.github.io/ambient-studio-site/terms.html`
- Data deletion: `https://<your-username>.github.io/ambient-studio-site/data-deletion.html`

## Where the links go

- **TikTok** (developers.tiktok.com → your app → Basic information): *Web/Desktop URL* = Home, *Terms of Service URL* = Terms, *Privacy Policy URL* = Privacy Policy.
- **Meta** (developers.facebook.com → your app → App settings → Basic): *Privacy Policy URL*, *Terms of Service URL*, and *User data deletion → Data deletion instructions URL* = Data deletion.
- **Google** (Cloud Console → OAuth consent screen / Branding): *Application home page*, *Application privacy policy link*, *Application terms of service link*.

## Changing them

The contact address is `ambient.studio.contact@gmail.com` on every page. Search and replace it if you use another. Section 12 of the Terms ("Governing law") names no place; you can put your state or country there. If you edit a page, change its "Effective" date.

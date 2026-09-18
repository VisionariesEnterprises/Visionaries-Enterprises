# Visionaries Enterprises — Website Files

This folder has everything you need to host the site yourself:

- **index.html** — the page itself (all photos are embedded directly in this file, so there's nothing extra to link up)
- **styles.css** — all the styling/design rules

## Hosting on GitHub Pages

1. Go to [github.com](https://github.com) and create a new repository (e.g. `visionaries-enterprises`). It can be public or private — GitHub Pages works with either on a paid plan, but the free plan requires the repo to be **public**.
2. On the repository page, click **Add file → Upload files**, then drag in `index.html` and `styles.css` from this folder. Commit the changes.
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment," set **Source** to "Deploy from a branch," pick the `main` branch and the `/ (root)` folder, then **Save**.
5. GitHub will give you a live link that looks like `https://yourusername.github.io/visionaries-enterprises/` within a minute or two.

## Connecting your own domain

Once the site is live on that GitHub link:

1. In the same **Settings → Pages** screen, enter your domain (e.g. `visionariesenterprises.com`) under "Custom domain" and save. GitHub will create a `CNAME` file in your repo automatically.
2. At your domain registrar (wherever you bought the domain — GoDaddy, Namecheap, etc.), add a **CNAME record** pointing your domain (or the `www` subdomain) to `yourusername.github.io`.
   - If you want the bare domain (`visionariesenterprises.com` with no `www`), GitHub's Pages docs list the specific **A records** to use instead of a CNAME — worth a quick look since the exact IPs can change.
3. DNS changes can take anywhere from a few minutes to a few hours to take effect.
4. Back in **Settings → Pages**, once GitHub detects the DNS is set up correctly, you can check **"Enforce HTTPS"** so the site loads securely.

That's it — no build steps, no server needed, just the two files above.

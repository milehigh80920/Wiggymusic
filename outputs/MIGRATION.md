# Wiggy Music site migration

## What this rebuild includes

This is a static, mobile-friendly rebuild of the public Wiggy Music site. It carries over the visible brand colors, the "Unforgettable live music for all occasions" positioning, the genres and booking occasions, the Desert Monks Brewing open mic schedule and description, the YouTube video, email, Venmo, Instagram, TikTok, and Chandler location.

The supplied square logo is assembled from the original file at `assets/wiggy-logo-original.jpeg`, with matching blue padding added in `assets/wiggy-logo-square.svg` to make the logo's overall visual spacing balanced. The original mark and lettering are unchanged. The touched-up hero banner from the live site—including its original photo and built-in Wiggy Music artwork—is saved as `assets/wiggy-banner.jpg` and displayed as a whole image, with no image filters or cropping. Keep these image files with the site when publishing.

GoDaddy's Websites + Marketing is a hosted builder. Its editor and publish workflow do not provide the normal editable HTML/CSS project that a static host can import; this migration is a rebuild based on the public site, not a direct export. The public page confirms the visible content, but not form submissions, hidden pages, analytics, or private builder data. Check the GoDaddy dashboard for any additional content and form submissions before disconnecting it.

## Recommended free hosting

**GitHub Pages** is the best fit for this site if you want to keep DNS at GoDaddy. It is free for a public repository and supports custom domains; after adding the domain to GitHub Pages, set the required apex A records and `www` CNAME at GoDaddy. [GitHub Pages custom-domain instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) · [GitHub Pages HTTPS](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https)

**Cloudflare Pages** is another free option. It works well with a custom apex domain, but requires the domain's nameservers to point to Cloudflare. Choose it if you prefer Cloudflare for DNS management. [Cloudflare custom-domain instructions](https://developers.cloudflare.com/pages/configuration/custom-domains/) · [Cloudflare Pages limits](https://developers.cloudflare.com/pages/platform/limits/)

The domain registration can remain at GoDaddy in either setup. Keep paying for the domain registration; the goal is to remove only the Website Builder/hosting product once the new site and email/DNS are verified. If GoDaddy hosts email for the domain, preserve its MX, SPF, DKIM, and DMARC records.

## Safe launch sequence

1. Preview the site with the included original logo and source photo. Check whether any other pages or content are missing from the public view.
2. Publish the files to the hosting provider's temporary preview URL first. Check all links, embedded video, mobile menu, contact email, HTTPS, and the page at a second device/browser.
3. Add the custom domain in the hosting dashboard before changing DNS. Save or screenshot the current GoDaddy DNS zone. Make only the web-hosting record changes required by your chosen provider. Do not remove mail records, domain registration, or unrelated records.
4. Confirm both `wiggymusic.com` and `www.wiggymusic.com` load the new site over HTTPS and that email still works. DNS may take time to propagate; keep the old builder active through this window.
5. Only after the replacement is stable, cancel the Website Builder product in GoDaddy. Confirm that domain registration and any email product remain active. Do not cancel the domain itself.

No account changes, purchases, DNS edits, or cancellations have been made.

# garrettmurphy.info

Personal site for Garrett Murphy. Static HTML — no build step, no framework, no dependencies.

## Hosting

### GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages → Source** → select `main` branch
3. The `CNAME` file handles the custom domain mapping
4. Add DNS records at your registrar (see below)

### Cloudflare Pages
1. Push this repo to GitHub
2. Go to [Cloudflare Dashboard → Pages](https://dash.cloudflare.com/?to=/:account/pages) → **Create a project**
3. Connect your GitHub repo
4. Build settings: **leave all fields blank** (no build command, output dir = `/`)
5. Add custom domain `garrettmurphy.info` in the Pages project settings

## DNS Records

### For GitHub Pages
```
Type    Name    Value
A       @       185.199.108.153
A       @       185.199.109.153
A       @       185.199.110.153
A       @       185.199.111.153
CNAME   www     YOUR-USERNAME.github.io
```

### For Cloudflare Pages
Cloudflare handles this automatically when you add the custom domain through the Pages dashboard.

## Local Preview
Just open `index.html` in a browser. No server needed.

## Structure
```
├── index.html    # Main page
├── 404.html      # Custom 404
├── CNAME         # GitHub Pages custom domain
└── README.md
```

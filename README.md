# KURA — Market Comps

Password-gated investor doc hosted at **kura.boahotels.com**.

## Stack
- Single static `index.html` — AES-GCM-encrypted comp content, PBKDF2-derived key (250,000 iterations), Web Crypto API decryption in-browser
- GitHub Pages from `main` branch, custom domain via CNAME

## Updating the content
1. Edit the master HTML in `Desktop/Claude/claude code /KURA copy/kura-market-comps.html`
2. Re-run `python3 /tmp/build_gated.py` to re-encrypt and rebuild `index.html`
3. Commit and push to `main`

## DNS setup (one-time)
At the boahotels.com DNS provider, add a CNAME record:
```
kura  →  lior-tech.github.io
```

## Access
- URL: https://kura.boahotels.com
- Access code: shared separately with investors

---
BOA Hotels &amp; Resorts · Confidential

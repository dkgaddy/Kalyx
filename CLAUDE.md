# Kalyx – PATRIA Biblical Family Tree

## Project
Single-file HTML app (`index.html`) using D3.js v7, PapaParse, and vanilla JS.
No build step required — edit `index.html` and deploy.

## Local Dev Server
```bash
python3 -m http.server 8082
```
Then open http://localhost:8082

## Deployment

**Live URL:** https://patria.explosiveconcepts.com

**Server:**
- Host: ssh.explosiveconcepts.com
- Port: 18765
- User: u303-2kknmnzzzr45
- SSH key: `~/.ssh/explosiveconcepts_key` *(must be present on the device — key is not stored in this repo)*
- Document root: `~/www/patria.explosiveconcepts.com/public_html`

**Deploy command** (git pull on server):
```bash
ssh -i ~/.ssh/explosiveconcepts_key -p 18765 u303-2kknmnzzzr45@ssh.explosiveconcepts.com \
  "cd ~/www/patria.explosiveconcepts.com/public_html && git pull"
```

To deploy, just tell Claude: **"deploy Kalyx"**

> Note: The SSH key passphrase is not stored anywhere — you will be prompted to enter it.
> To avoid repeated prompts in a session, run `ssh-add ~/.ssh/explosiveconcepts_key` first.

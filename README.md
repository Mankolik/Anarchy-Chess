
# Chess P2P (no server)

Single-file chess for the browser with **uniform SVG pieces**, full rules, and **online multiplayer via WebRTC DataChannel** — **no servers** required. Signaling is done manually by copy/paste or QR.

## Features
- Legal move generation: check, checkmate, stalemate, castling, en passant, promotions (Q/R/B/N)
- Clean SVG piece set (cburnett)
- P2P online play over WebRTC (end-to-end between browsers)
- Manual signaling: share an Offer and Answer via text or QR (no backend)
- Mobile-friendly UI

## Quick start
1. Open `index.html` locally in any modern browser, or publish via GitHub Pages (below).
2. Click **Host online** → copy the Offer (or show QR) to your friend.
3. Friend clicks **Join online** → pastes your Offer → sends you their Answer (or QR).
4. You paste the Answer and press **Connect**. Play!

> Tip: If you sit behind a very restrictive NAT, a TURN relay may be required (not included). Most home networks work with public STUN only.

## Publish on GitHub Pages
1. Create a new repo (e.g. `chess-p2p`) on GitHub.
2. Upload `index.html` to the root of the repo and commit.
3. Go to **Settings → Pages**.
4. **Build and deployment**: choose **Deploy from a branch**.
5. Select **Branch: `main`** and **Folder: `/ (root)`**. Save.
6. Your site will appear at `https://<your-username>.github.io/<repo-name>/`.

## Local development (optional)
```bash
# one-time setup
git init -b main
git add index.html
git commit -m "Initial commit: chess p2p (no server)"
git remote add origin https://github.com/<you>/chess-p2p.git
git push -u origin main
```

## License
[MIT](LICENSE)

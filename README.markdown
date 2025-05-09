# Trembyle: A Zork Game

Trembyle is a browser-based, text-adventure game set in the Zork universe, where you play as Wizard Trembyle in 1247 GUE, tasked with casting the Great Diffusion to defeat evil magic. This project is a single-page web application using React, Tailwind CSS, and a custom JavaScript game engine.

## Files
- `index.html`: The complete game, including UI and logic.
- `README.md`: This file with setup instructions.

## Setup Instructions

### Prerequisites
- A web browser (e.g., Chrome, Firefox) to run the game.
- (Optional) Node.js and npm for local testing with a server.
- A web server or hosting service (e.g., Netlify, Vercel) for deployment.

### Local Testing
1. **Save Files**:
   - Place `index.html` in a directory (e.g., `trembyle`).
2. **Run a Local Server**:
   - Install Node.js (https://nodejs.org) if not already installed.
   - Open a terminal in the `trembyle` directory and run:
     ```
     npx http-server
     ```
   - Open `http://localhost:8080` in your browser.
3. **Play**:
   - Enter commands like `look`, `go north`, `take crystal`, `talk to canuk`, or `cast diffusion`.
   - See the game’s tip for more commands.

### Deployment
1. **Host the Files**:
   - Upload `index.html` to a static hosting service (e.g., Netlify, Vercel) or a web server (e.g., Nginx, Apache).
   - For Netlify:
     - Drag and drop the `trembyle` folder to Netlify’s dashboard (https://app.netlify.com).
     - Deploy and get a URL (e.g., `https://your-site.netlify.app`).
   - For a custom domain (trembyle.com):
     - Update your domain’s DNS to point to the hosting provider.
     - Configure the server to serve `index.html`.
2. **Enable HTTPS**:
   - Use a certificate (e.g., Let’s Encrypt) for secure access.
3. **Access**:
   - Visit `https://trembyle.com` (or your deployed URL) to play.

### Dependencies
- The game uses CDN-hosted libraries (loaded in `index.html`):
  - React and React DOM (`18.2.0`)
  - Tailwind CSS
  - Babel (`7.22.5`) for JSX
- No local dependencies or backend required.

## Gameplay
- **Objective**: Collect the Crystal of Illumynite, Scroll of Deception, and Orb of Longevity, then cast the Great Diffusion in the Illumynite Caverns.
- **Locations**: Illumynite Caverns, Library, Vault.
- **Puzzles**:
  - Take the Crystal (`take crystal`).
  - Get the Scroll (`go north`, `take scroll`).
  - Talk to Canuk (`talk to canuk`) to defeat Malveo, then take the Orb (`go east`, `take orb`).
  - Cast the spell (`cast diffusion`) with all items.
- **Commands**:
  - `look`: Describe the current room.
  - `go [direction]`: Move (e.g., `go north`).
  - `take [item]`: Pick up an item (e.g., `take crystal`).
  - `inventory`: List carried items.
  - `talk to canuk`: Interact with Canuk.
  - `cast diffusion`: Cast the final spell.

## Notes
- The game is a static site, requiring no server-side logic.
- Ensure `index.html` is served over HTTP/HTTPS to load CDN resources.
- For issues, check the browser console for errors (e.g., CORS issues if testing without a server).

Enjoy playing Trembyle!
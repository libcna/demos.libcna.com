CNA House 1.1.0 for the Web

Serve this directory from any static HTTP server and open index.html, for example:

    python3 -m http.server 8000     # then http://localhost:8000/

The server must send .wasm as application/wasm; gzip or brotli compression of the .data.part* files and .wasm can reduce
the download size. A WebGL 2 browser is required (tested: Chrome 152 and
Firefox 140 ESR). The first click or key press starts audio, as browsers require.

Limitations: settings apply for the session and are not kept across a reload; if the browser
loses the WebGL context (a driver reset, for example), reload the page.

The programme is Ms-PL (LICENSE); runtime notices are in NOTICE.md and every content asset's
author and licence is in licenses/THIRD-PARTY-ASSETS.md.

For this GitHub Pages deployment, cna-house.data is split into four numbered parts;
cna-house.js streams them in order when the demo starts. Keep all four parts together.

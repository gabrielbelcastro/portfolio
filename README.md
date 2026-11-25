# Portfolio: Gabriel Belcastro

Voice AI, agents and automation. Self-contained static pages, no build step, vanilla JS, PT/EN toggle.

Design: airport-wayfinding signage (sign black, signal yellow, concourse grey; Barlow Condensed and Barlow). See `DESIGN.md`.

**Live:** https://gabrielbelcastro.labsaero.com/ (canonical). https://portfolio.labsaero.com/ keeps working: it is the GitHub Pages domain in `CNAME`, and the canonical address proxies it.

## Pages
- `index.html`: home. Opens with the voice AI work: a player with a test call by Clara, the Domus voice assistant (`audio/clara-ligacao-de-teste.mp3`, 1:42, fictitious data, simulated agent), how the call center works and the full transcript. Then the Domus ecosystem, the Labs Aero tools, more projects, about and contact.
- `miles-terminal.html`: case page for Miles Terminal (screenshots with no data, modules, stack). The terminal itself needs an authorized Google login.
- `capturador-azul.html`: case page for Capturador Azul, the Domus ticketing team's Chrome extension.
- `og.jpg`: social preview image (1200x630).

## Links out
- Domus call center (voice agent): https://domuspi.com.br/central-de-atendimento.html
- Domus dashboard demo (fictitious data): https://domuspi.com.br/demonstracao.html
- Domus website: https://domuspi.com.br/servicos.html
- Capturador Smiles on the Chrome Web Store, labsaero.com, viajagencia.com.br, LinkedIn, GitHub

## i18n rule
Elements with `data-pt` hold text only (the script swaps `textContent`), never child elements.

## Contact
- Email: gabrielbelcastro.contatos@gmail.com
- LinkedIn: https://www.linkedin.com/in/gabrielbelcastro

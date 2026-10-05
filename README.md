# Orbital Logistics

A browser-based space freight trading game. You run mission control for a small shipping company in the year 2040, buying goods where they're cheap and flying them across the solar system to where they sell high, using real orbital mechanics to plan every transfer.

## Features

- **Real orbital mechanics.** Planets follow circular Keplerian orbits. Transfers are solved with a Lambert solver, and fuel use comes from the Tsiolkovsky rocket equation, Oberth-effect departure and capture burns, and aerobraking at worlds with an atmosphere.
- **Porkchop plots.** Each route shows a Δv chart of departure date against flight time, so you can see when the launch windows open.
- **A living economy.** Nine worlds (Mercury through Neptune, plus the Moon) and 13 launch sites each sell and buy their own goods. Prices move with your trades (big orders pay more per tonne), local industry restocks over time, economies drift, news events spike or crash markets, and the colonies grow.
- **A Markets screen.** Every price at every world, price-history charts, a ranked route finder, and recent news.
- **Realistic cargo.** 13 goods in five tiers. Food and medicine spoil and cryogenic cargo boils off on long flights.
- **Contracts.** Deliver a good to a world by a deadline for a premium, or pay a penalty.
- **Loans and bases.** Start in debt, borrow against your fleet, and build orbital depots (no lift fee), trading posts (cheaper goods), and warehouses (store cargo). Miss a loan payment and the lender seizes ships.
- **Rival companies.** Two AI freight companies fly by the same rules, compete in the same markets, and grow their fleets. Compare net worth in the standings.
- **A fleet to manage.** Fly chemical-nuclear *Haulers* (40 t cargo) for the inner system and fusion *Clippers* (20 t) for the outer planets, and buy more ships as you grow.
- **Flight timelines.** Each flight lists its burns, sphere-of-influence crossings, perihelion and aphelion, and planetary orbit crossings.
- **A finance dashboard.** Track your balance history, income and spending, profit per ship, loans, standings, and every transaction.
- **Playable on phones.** The phone layout has a full-screen map, bottom-sheet panels, touch and pinch controls, and larger tap targets.
- **Saves.** The game autosaves to browser storage every 5 seconds, and you can export or import a save as a JSON file.

## Running it

The whole game is one file, `index.html`, with no dependencies and no build step.

```sh
git clone https://github.com/kefortney/orbital_logistics.git
cd orbital_logistics
# open index.html in a browser, or serve it:
python3 -m http.server 8000   # then visit http://localhost:8000
```

It works in desktop browsers and on phones. On narrow screens the panels move into a bottom tab bar, and the map supports touch panning and pinch-to-zoom.

To host it, enable GitHub Pages on the `main` branch, root folder.

## How to play

See **[HOW_TO_PLAY.md](HOW_TO_PLAY.md)** for a full guide, or press `?` in the game.

## Project layout

| File | Purpose |
|------|---------|
| `index.html` | The whole game: HTML, CSS, and JavaScript (physics, economy, rivals, rendering, UI, saves) |
| `HOW_TO_PLAY.md` | Player guide |

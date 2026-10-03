# Orbital Logistics

A browser-based space freight trading game. You run mission control for a small shipping company in the year 2040, buying goods where they're cheap and flying them across the solar system to where they sell high, using real orbital mechanics to plan every transfer.

## Features

- **Real orbital mechanics.** Planets follow circular Keplerian orbits. Transfers are solved with a Lambert solver, and fuel use comes from the Tsiolkovsky rocket equation, Oberth-effect departure and capture burns, and aerobraking at worlds with an atmosphere.
- **Porkchop plots.** Each route shows a Δv chart of departure date against flight time, so you can see when the launch windows open.
- **A dynamic economy.** Nine worlds (Mercury through Neptune, plus the Moon) and 13 launch sites each sell and buy their own goods. Your trades move prices, and markets recover over time.
- **A fleet to manage.** Fly chemical-nuclear *Haulers* (40 t cargo) for the inner system and fusion *Clippers* (20 t) for the outer planets, and buy more ships as you grow.
- **Flight timelines.** Each flight lists its burns, sphere-of-influence crossings, perihelion and aphelion, and planetary orbit crossings.
- **A finance dashboard.** Track your balance history, income and spending, profit per ship, and every transaction.
- **Saves.** The game autosaves to browser storage every 5 seconds, and you can export or import a save as a JSON file.

## Running it

The whole game is one file, `index.html`, with no dependencies and no build step.

```sh
git clone https://github.com/kefortney/orbital_logistics.git
cd orbital_logistics
# open index.html in a browser, or serve it:
python3 -m http.server 8000   # then visit http://localhost:8000
```

The layout is designed for a desktop browser.

## How to play

See **[HOW_TO_PLAY.md](HOW_TO_PLAY.md)** for a full guide, or press `?` in the game.

## Project layout

| File | Purpose |
|------|---------|
| `index.html` | The whole game: HTML, CSS, and JavaScript (physics, economy, rendering, UI, saves) |
| `HOW_TO_PLAY.md` | Player guide |

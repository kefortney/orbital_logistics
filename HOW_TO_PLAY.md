# How to Play Orbital Logistics

You run mission control for a freight company. The game starts on 1 January 2040, and you have **$3.00M**, three Haulers, and one Clipper. Grow your money by trading goods between worlds.

## The goal

Every world **sells** some goods cheaply and **buys** others at a premium. Buy low, fly, and sell high. When a ship arrives, any cargo the destination buys is **sold automatically**. Anything that world doesn't buy stays aboard for the next leg.

There is no fixed win condition. The aim is to build the most profitable fleet you can.

## The screen

| Area | What it shows |
|------|---------------|
| **Top bar** | Date, money (click it for the finance dashboard), time speed, inner/outer view, pause-on-arrival toggle, help (`?`), and game/save menu |
| **Flight Board** (left) | Your ships with their status, location, and cargo. Click a ship to plan or inspect it. The buy-ship controls are at the bottom. |
| **Planet panel** (left) | The selected world's sites, propellant price, what it sells and buys (with live price trends), and docked ships. Switch worlds with the MER/VEN/EAR… buttons. |
| **Log** (bottom left) | Recent launches, arrivals, and sales |
| **Map** (center) | The solar system. Click planets or ships to follow them. |
| **Planner** (right) | Opens when you select a ship |

## Flying a cargo run

1. **Pause** with `Space` so you can plan calmly.
2. **Click a docked ship** on the Flight Board.
3. **Pick a destination** from the `TO` dropdown. Each option shows what your current manifest would sell for there. You can also click a planet and press **"send <ship> here"** next to one of its sites.
4. **Load cargo** with the `−` / `+` buttons (5 t per click; **shift-click** to fill or empty). The table shows the price here and the price at the destination. A dash means the destination doesn't buy that good.
5. **Choose a transfer window** on the porkchop chart:
   - **x-axis:** departure date (from now to roughly one synodic period ahead)
   - **y-axis:** flight time
   - **Bright green** means cheap Δv (little fuel), **red/brown** means expensive, and **dark** means the ship can't carry enough fuel with this load.
   - Click the chart to select a window. The planner picks a good early one for you automatically.
6. Check the readout (cost, revenue, profit, Δv, fuel). Tick **fill tank** to top up completely, which is useful where propellant is cheap.
7. Press **SCHEDULE LAUNCH**. The ship launches on its departure date and you can watch it fly. Expand the flight plan to see the event timeline: burns, sphere-of-influence crossings, apsides, and orbit crossings.

With **pause on arrival** checked, the game pauses whenever a ship arrives, so none of your ships sits idle.

## Ships

| Class | Price | Cargo | Tank | Drive | Best for |
|-------|-------|-------|------|-------|----------|
| **Hauler** | $2.00M | 40 t | 80 t | Nuclear thermal (exhaust 7.85 km/s) | Earth, Moon, Mars, Venus |
| **Clipper** | $6.00M | 20 t | 60 t | Fusion (exhaust 20 km/s) | Mercury and the outer planets |

To buy a ship, choose a class and a starting site at the bottom of the Flight Board, then press **buy**.

## Costs

- **Cargo:** the purchase price at the departure world.
- **Propellant:** the local price per tonne. It's very cheap at the Moon (Shackleton) and at the gas-giant stations, and expensive at Mercury and Venus.
- **Lift fee:** charged per tonne launched (ship + cargo + fuel). Surface sites charge the most (Earth around $2.4–3.0k/t). Orbital stations charge almost nothing.

**Aerobraking:** Earth, Venus, Mars, and the gas giants let you use the atmosphere to slow down, so arriving there costs far less fuel. Mercury and the Moon have no atmosphere, so you pay the full capture burn.

## The market

- Prices are in **$k per tonne**.
- Buying pushes a world's price **up**, and selling pushes it **down**. Small, specialist goods (helium-3, samples) move fastest.
- Prices drift back to normal over a few months. The planet panel shows ▲/▼ percentages when a price is off its baseline.
- Spread your trades across routes rather than flooding one market.

### Where things come from and where they go

| World | Sells (you buy) | Buys (you sell) |
|-------|-----------------|-----------------|
| Mercury | solar cells, metals | water, food, machinery, electronics |
| Venus | chemicals, samples | water, metals, food, electronics, machinery |
| Earth | food, machinery, electronics | helium-3, samples, metals, solar cells, deuterium, chemicals |
| Moon | water, propellant, metals, helium-3 | food, machinery, electronics, solar cells |
| Mars | samples, metals, water | food, machinery, electronics, propellant, volatiles, chemicals |
| Jupiter | helium-3, deuterium, propellant | food, machinery, electronics, water, metals |
| Saturn | volatiles, helium-3, propellant | food, machinery, electronics, metals, solar cells |
| Uranus | deuterium, volatiles, propellant | food, electronics, machinery, solar cells |
| Neptune | deuterium, volatiles, samples, propellant | food, electronics, machinery, solar cells |

Each launch site only stocks some of its world's goods. Check the site list in the planet panel.

## Tips for getting started

- **Earth ↔ Moon** is a short, cheap loop. Take electronics or machinery up, and bring helium-3 (sells at about $90k/t on Earth) back from Imbrium.
- **Mars samples** sell for about $70k/t on Earth. Earth electronics sell for about $40k/t on Mars, so a Hauler can carry paying cargo both ways.
- The **outer planets** pay huge prices for food, machinery, and electronics, but trips take years. Send Clippers, fill their tanks cheaply at the stations, and bring back helium-3 or deuterium.
- **Wait for a window.** Launching on the bright green part of the porkchop plot can cut fuel costs dramatically.
- Open the **finance dashboard** (click your money) to see which ships and routes actually make a profit.

## Controls

| Input | Action |
|-------|--------|
| Mouse wheel / zoom slider | Zoom |
| Drag | Pan |
| Click a planet or ship | Follow it / open it |
| `1` | Inner system view |
| `0` | Outer system view |
| `Space` | Pause / resume |
| `+` / `-` | Speed up / slow down (1 to 365 days per second) |
| `?` | Help |
| `Esc` | Close the dialog or planner |

## Saving

The game **autosaves every 5 seconds** to your browser's local storage. Open **game / save** to:

- **save now**
- **save to file…** to export a JSON backup (browser saves are lost if you clear site data or switch browsers)
- **load from file…** to import a backup
- **new game** to start over

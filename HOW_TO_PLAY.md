# How to Play Orbital Logistics

You run mission control for a freight company. The game starts on 1 January 2040. You have **$7.00M** in cash, three Haulers, one Clipper, and a **$4.00M loan** due in two years. Grow your company by trading goods between worlds, and pay the loan back before it falls due.

## The goal

Every world **sells** some goods cheaply and **buys** others at a premium. Buy low, fly, and sell high. When a ship arrives, any cargo the destination buys is **sold automatically**. Anything that world doesn't buy stays aboard for the next leg.

There is no fixed win condition. Two rival companies trade by the same rules. The aim is to build a bigger company than theirs, measured by **net worth**: cash, minus debt, plus your ships and bases at resale value.

## The screen

| Area | What it shows |
|------|---------------|
| **Top bar** | Date, money (click it for the finance dashboard), debt, time speed, inner/outer view, rival ships on/off, auto-pause, **markets**, help (`?`), and game/save menu |
| **Flight Board** (left) | Your ships with their status, location, and cargo. Click a ship to plan or inspect it. The buy-ship controls are at the bottom. |
| **Planet panel** (left) | The selected world's news, sites and your bases there, propellant price, what it sells and buys (with price trends and how fast it makes or uses each good), and docked ships. Switch worlds with the MER/VEN/EAR… buttons. |
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

With **auto-pause** checked, the game pauses whenever a ship arrives, a loan is about to fall due, or a contract is missed.

To sell a docked ship, use the button at the bottom of its planner. It fetches 60% of its price, and any cargo aboard is lost.

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

Prices are in **$k per tonne**. Every world has a normal price for each good it trades. Four things move a price away from it:

- **Trade.** Buying pushes a world's price **up**, and selling pushes it **down**. The price moves as the order fills, so a big order pays more per tonne than a small one. Small, specialist goods (helium-3, samples, medicine) move fastest.
- **Local industry.** Each world makes back what traders took, or uses up what they delivered, at a steady rate. The planet panel shows the rate, for example "makes 2.8 t/d" or "uses 0.4 t/d". Take 40 t of helium-3 from the Moon and it takes a couple of months to recover.
- **Drift.** Every local economy wanders slowly, typically about 15% either side of normal over a year or two.
- **News.** Every few months, an event spikes or crashes one market, such as a crop failure on Mars or a chip glut on Earth. The effect fades over months. News appears in the log, the planet panel, and the Markets screen.

Markets also **grow**. The colonies on Mars, the Moon, and the outer planets grow by 3–6% a year, so they absorb bigger deliveries without the price collapsing. Earth is huge from the start.

Rival ships trade in the same markets, so a spread you are counting on can close before your ship arrives. Spread your trades across routes rather than flooding one market.

### The Markets screen

Press **markets** in the top bar.

| Tab | Shows |
|-----|-------|
| **prices** | Every good at every world. **Green** prices are goods you can load there, and **amber** prices are goods the world buys. ▲/▼ marks a price off its normal level. Click a good to chart its price history at every world (log scale; hover to compare). Recent news is listed below. |
| **routes** | The most profitable runs at today's prices for a Hauler or a Clipper, from anywhere or from one world. It shows the load, flight time, Δv, profit per trip, profit per 30 days, and which of your ships are already there. These are estimates for a Hohmann transfer, and the planner's chart shows the real windows. |
| **contracts** | Your contracts and the open offers (see below). |

### Goods

| Kind | Goods |
|------|-------|
| Raw materials | water, volatiles, helium-3 |
| Refined | metals, propellant, deuterium, chemicals |
| Manufactured | solar cells, machinery, electronics |
| Consumer goods | food, medicine |
| Research | samples |

Some cargo doesn't survive long flights intact. **Food** spoils (10% a year), **medicine** loses 5% a year, and cryogenic **helium-3**, **deuterium**, and **propellant** boil off at 2–3% a year. The planner shows the rate next to the good and how much you would lose on the selected flight. This matters most on multi-year runs to the outer planets.

### Contracts

Every few weeks a world posts an offer, for example "deliver 30 t of medicine to Mars by 2043-06-01" at a rate well above the market price. Accept it on the Markets screen (you can hold up to four at once). Then deliver the goods to any site on that world, in as many trips as you like. Each tonne pays the contract rate on arrival, before the market buys the rest. The planner marks contract destinations with ★.

If the deadline passes with goods still owed, you pay **25% of the undelivered value** as a penalty. Rivals take open offers too, so an offer can disappear before it expires.

## Loans

You start with a **$4.00M loan due in two years**. Interest is charged monthly. Manage loans from the finance dashboard (click your money):

- **Borrow** $1M, $2M, or $5M for 1, 2, or 5 years. Lenders advance up to 70% of what your ships and bases cost (your **credit limit**). The rate rises with the term and with how much of your limit you have used.
- **Repay** early, $1M at a time or in full.
- When a loan falls due it is **repaid automatically** if you have the cash. If you don't, you're warned 60 days ahead.
- **Missing the due date** adds a 10% late fee, raises the rate by 4 points, and gives you 180 more days. **Missing that** makes the lender seize your docked ships, most valuable first, and sell them at 60% of their price until the loan is covered.
- A **negative balance** is charged overdraft interest at 20% a year.

## Bases

Build bases from the planet panel. Press **build…** next to a site. Each costs a one-off price plus monthly upkeep:

| Base | Effect | Cost | Upkeep |
|------|--------|------|--------|
| **Orbital depot** | No lift fee on your launches from that site (not at orbital stations, which barely charge one) | $1M + $0.8M × the site's lift fee | $30k/month |
| **Trading post** | 20% off the goods you buy at that site | $2.5M | $25k/month |
| **Warehouse** | Store cargo there between flights. In the planner, **+** loads into the hold and **−** stores. Stored goods the world buys can be sold from the planet panel at any time. | $1.5M | $10k/month |

A depot at Kennedy saves up to about $400k on every Hauler launch. A warehouse at the Moon lets you stockpile helium-3 and sell it when Earth's price peaks.

## Rivals

**Ceres Freight** (purple) and **Helios Haulage** (pink) fly the same ships under the same rules: same prices, fuel, fees, and transfer windows. Each idle ship takes the most profitable run per day it can find. Their trades move the same markets yours do, and they buy more ships as they earn. Their ships appear on the map as small coloured arrows. Click one to see where it's going, or press **rivals** in the top bar to hide them. The **standings** on the finance dashboard compare everyone's net worth.

### Where things come from and where they go

| World | Sells (you buy) | Buys (you sell) |
|-------|-----------------|-----------------|
| Mercury | solar cells, metals | water, food, machinery, electronics, medicine |
| Venus | chemicals, samples, medicine | water, metals, food, electronics, machinery |
| Earth | food, machinery, electronics, medicine | helium-3, samples, metals, solar cells, deuterium, chemicals |
| Moon | water, propellant, metals, helium-3 | food, machinery, electronics, solar cells, medicine |
| Mars | samples, metals, water | food, machinery, electronics, propellant, volatiles, chemicals, medicine |
| Jupiter | helium-3, deuterium, propellant | food, machinery, electronics, water, metals, medicine |
| Saturn | volatiles, helium-3, propellant | food, machinery, electronics, metals, solar cells, medicine |
| Uranus | deuterium, volatiles, propellant | food, electronics, machinery, solar cells, medicine |
| Neptune | deuterium, volatiles, samples, propellant | food, electronics, machinery, solar cells, medicine |

Each launch site only stocks some of its world's goods. Check the site list in the planet panel.

## Tips for getting started

- **Open the Markets screen first.** The routes tab ranks today's best runs for each ship class.
- **Earth ↔ Moon** is a short, cheap loop. Take electronics or medicine up, and bring helium-3 (sells at about $90k/t on Earth) back from Imbrium.
- **Mars samples** sell for about $70k/t on Earth. Earth electronics sell for about $40k/t on Mars, so a Hauler can carry paying cargo both ways.
- The **outer planets** pay huge prices for food, machinery, and electronics, but trips take years. Send Clippers, fill their tanks cheaply at the stations, and bring back helium-3 or deuterium.
- **Wait for a window.** Launching on the bright green part of the porkchop plot can cut fuel costs dramatically.
- Open the **finance dashboard** (click your money) to see which ships and routes actually make a profit.
- **Plan for the loan.** $4M falls due at the end of 2041. Either keep enough cash, or refinance with a longer loan before the due date.
- **Contracts pay well** but tie you to a deadline. Accept ones you can reach in time, ideally with a ship already near a source of the good.

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

### On a phone

The game works on phones and tablets in a browser. On narrow screens the map fills the screen, and the panels appear as a sheet above a tab bar at the bottom:

| Tab | Shows |
|-----|-------|
| **FLEET** | The flight board and the buy-ship controls |
| **PLANET** | The selected world's sites and prices. Tapping a planet on the map opens this tab. |
| **SHIP** | The planner or flight log for the selected ship. Tapping a ship opens this tab. |
| **LOG** | Recent events |

Tap the open tab again to hide the sheet and see the whole map.

- **Drag** to pan and **pinch** to zoom the map.
- On the transfer chart, **tap** a spot to pick that window, or **drag** across the chart to preview windows and lift your finger on the one you want.
- Use **max** next to a cargo row to fill the hold, since there is no shift key.
- On the finance charts, tap or drag sideways to see values.
- To play full screen, **install** the game: in Chrome, open the menu and choose **Install app** (or **Add to Home screen**). On an iPhone, use Safari's **Share → Add to Home Screen**. The installed game has its own icon, opens full screen, and works offline.

Browser saves are separate for each device. To move a game between your phone and computer, use **save to file** and **load from file**.

## Saving

The game **autosaves every 5 seconds** to your browser's local storage. Open **game / save** to:

- **save now**
- **save to file…** to export a JSON backup (browser saves are lost if you clear site data or switch browsers)
- **load from file…** to import a backup
- **new game** to start over

Saves from earlier versions of the game load and are upgraded automatically. Your ships, money, and history carry over, the rivals join, and you start without a loan.

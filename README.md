# Modular Storage Configurator

A web configurator for a modular pole-and-plank storage / shelving system.
Customers set dimensions and materials, drag shelf levels to any height,
click between poles to place planks, see a live price estimate, and send a
quote request.

## Features
- **Dimensions** — width, height, depth, plank thickness (mm) with live dimension lines.
- **Structure** — number of poles (columns), shelf levels (rows), pole diameter, shepherd's-crook tops.
- **Drag-to-position rows** — drag the ⇕ handle on any level to set its exact height.
- **Click-to-place planks** — click a cell between two poles to add/remove a shelf; adjacent planks merge.
- **Materials** — six plank woods and four pole finishes, each priced.
- **Add-ons** — rolling drawer cabinet and a deeper desk worktop.
- **Live pricing** + full breakdown, JSON export, and an email quote-request form.

## Running
It's a single static file — just open `index.html`, or serve the folder.

## Configuration
- Change `QUOTE_EMAIL` near the top of the `<script>` in `index.html` to the address
  that should receive quote requests.
- Material and finish prices live in the `WOODS` and `POLE_FINISHES` arrays.

## Deploy
Static site — deploys to Vercel (or any static host) with no build step.

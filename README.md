# Audi Charging Time Simulator (prototype)

An interaction demo of the Audi charging time simulator. It shows how the screen looks and responds, so the live tool can be compared with the design. It is not production code.

## Open it
Open `index.html` in a browser. There is nothing to install or build, and it works offline.

## Files
| File | What it is |
|---|---|
| `index.html` | The default page, as on the live tool |
| `index-section-group.html` | Work in progress, needs further development: result section with call-to-action buttons, in the "Section Group" layout the client prefers (buttons in their own card). Figma: page `[Range] Add Next Step CTAs`, section "Section Group (Client Preferred)". |
| `assets/` | Fonts, icons and model images |

## What you can try
- Choose where you charge (home, workplace, public, motorway), the charger type and the charging power (2.3, 7.2, 50, 150 or 350 kW).
- Move the two handles to set the current and the desired charge.
- Set the outside temperature and whether the station is approached with route guidance. The estimated charging time updates straight away.
- Click the (i) buttons for an explanation. `Esc` or a click outside closes it.
- Open the FAQ rows (one at a time).
- Make the window narrower than 1024 px to see the result bar stick to the bottom of the screen.

## Design reference
Figma, page `[All] Ready for Dev`, section "Charging Time" (six frames: 320, 375, 768, 1024, 1440, 1920).

## Good to know
- Colours, type and spacing come from the DS3 Web UI Kit 2.1 tokens. They are the `--sys-*` custom properties at the top of the file; change a value there, not in the rules below.
- Copy is English (UK), with the five UK power steps. The German live page has seven.
- The calculation and selection logic (for example which options are disabled) is simplified and not the production logic. Accessibility is out of scope.
- The top bar imitates the live Audi header for context.

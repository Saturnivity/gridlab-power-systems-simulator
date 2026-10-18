# GridLab — Interactive DC Circuit Simulator

A self-contained browser-based educational simulator for resistive DC circuits. Built using vanilla HTML, CSS, and JavaScript; no dependencies or backend required.

## Features
- Interactive voltage (1–48 V), resistance (1–100 Ω), operating time (1–24 h), and energy tariff controls
- Real-time Ohm's law, electrical power, energy and cost calculations
- Dynamic SVG circuit diagram and power-vs-resistance graph
- CSV export for scenario analysis
- Responsive layout, accessible form labels, and stated model assumptions

## Run
Open `index.html` in a modern browser. No installation required.

## Engineering model
For an ideal constant-voltage DC source with a single linear resistor:
- Current: `I = V/R` (amperes)
- Power: `P = VI = V²/R` (watts)
- Energy: `E = P × t / 1000` (kWh, when t is in hours)
- Cost: `cost = E × rate` (USD)

Example: 24 V across 12 Ω produces 2 A, 48 W, and 0.384 kWh over 8 hours. At $0.18/kWh, the energy costs $0.06912.

## Limitations
This is an idealized educational model. It does not model transients, reactive loads, source impedance, component tolerances, thermal effects, protection devices, or wiring losses. Do not use it to size or validate real electrical installations.

## Suggested extensions
Add series/parallel resistor networks, circuit fault detection, component thermal constraints, unit tests, and historical scenario comparison.

## Attribution
Initial project scaffold and implementation generated with AI assistance. Review, test, and extend before representing this work as independent engineering experience.

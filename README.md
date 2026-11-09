# Air Cycle Explorer

An interactive, browser-based tool for exploring the air-standard power cycles studied in applied thermodynamics. Each cycle is shown side by side with a rotatable 3D model of the machine that runs it, so you can see how the hardware and the thermodynamics line up.

**Live site:** https://yashyrrbas-pixel.github.io/air-cycle-explorer/

## Features

- **Five cycles:** Otto, Diesel, Dual, Brayton and Carnot, with adjustable inputs (compression ratio, cut-off ratio, pressure ratio, peak temperature, reservoir temperatures and more).
- **3D state space:** each cycle is drawn on the ideal-gas surface in P–v–T or T–s–P space. You can rotate it freely or snap it to the classic P–v and T–s views.
- **3D machines, synced to the cycle:**
  - Four-stroke petrol engine with spark plug and timed valves (Otto)
  - Diesel engines with fuel injector and spray (Diesel, Dual)
  - Gas turbine with spinning compressor and turbine and temperature-coloured gas flow (Brayton)
  - Piston–cylinder with sliding hot and cold reservoirs (Carnot)
- **Live readouts:** crank angle, volume, pressure and temperature, plus a P–V indicator diagram that tracks the piston.
- **Otto engine calculator:** enter bore, stroke, cylinders, speed and operating conditions to get displacement, cycle states, efficiency, mean effective pressure, indicated power and torque, with a step-by-step worked solution.
- **Formula sheet:** every relation used, grouped by topic, with a table of symbols.
- **Built-in glossary:** point at or tap any underlined term to read its definition and practical uses.

## Assumptions

The calculations use the cold-air standard: air as an ideal gas with R = 0.287 kJ/kg·K, γ = 1.4, cp = 1.005 kJ/kg·K and cv = 0.718 kJ/kg·K. All processes are internally reversible. The results are ideal indicated values. Real engines produce less because of heat loss, friction, pumping work and specific heats that vary with temperature.

## Tech

A single self-contained `index.html` using plain JavaScript, [three.js](https://threejs.org/) (r128) for the 3D views and the Canvas 2D API for the live plots. There is no build step: open `index.html` in a browser, or serve the folder with any static host.

## Author

[yashyrrbas-pixel](https://github.com/yashyrrbas-pixel)

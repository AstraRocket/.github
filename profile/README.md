# AstraRocketSim

**Model rocket design and flight simulation, in the browser, on real OpenRocket physics.**

AstraRocketSim is the home of an open source rocketry simulator that runs entirely on your device. Design a rocket, watch its center of gravity, center of pressure, and stability update as you edit, pick a real motor, and fly a full simulation. Nothing to install, nothing uploaded, and it keeps working offline once loaded.

**[Launch the app](https://AstraRocket.github.io/simulator/)** · **[Documentation](https://AstraRocket.github.io/simulator/docs/)** · **[Safety](https://AstraRocket.github.io/simulator/docs/safety)**

## What lives here

| Repository | What it is |
| --- | --- |
| **[AstraRocket Simulator](https://github.com/AstraRocket/simulator)** | The simulator: the web app plus the OpenRocket engine build it runs on. |

The app is a lightweight, mobile friendly interface over the OpenRocket core, not a re-creation of the desktop program. It reads and writes OpenRocket `.ork` files at full fidelity, imports and exports RockSim `.rkt`, and exports design reports, 3D models, cut sheets, flight data, and flight paths.

## Why it exists

- **Trusted physics.** The engine is the actual OpenRocket core (extended Barrowman aerodynamics with opt-in RASAero supersonic extensions, mass and CG, RK4 flight integration), compiled to WebAssembly and validated bit-identical to upstream.
- **Runs anywhere.** Desktop, tablet, or phone. A three-pane workbench on a wide screen becomes tabs on a small one.
- **Yours, on your device.** No server, no accounts. Designs are files on your disk. The browser keeps a working copy, your custom motors, materials, and settings.
- **Limits.** Launch conditions are held to NAR and Tripoli flying limits, as well as not modeling: fin flutter, structural loads, parachute opening shock, and how your motor behaves on the day.

## Features at a glance

- Component tree editor with live CG, CP, and stability margins, on the pad and at rail exit
- Multi-stage rockets with boosters, pods, and parallel staging
- 2D schematic with calipers and rulers, 3D model view, aerodynamics view, flight charts, and a 3D flight path
- Real thrust curves for roughly 800 motors from thrustcurve.org, plus `.eng` import and custom motors
- OpenRocket materials and a catalog of roughly 2,900 real component presets
- Per-component aerodynamic analysis matching desktop OpenRocket's Component Analysis
- Exports to PDF, CSV, RASAero II, STL, OBJ, GLB, 3MF, DXF, SVG, PNG, KML, and GPX
- Undo and redo across the whole workspace
- Metric, imperial, or a unit of your choice per quantity
- Multilingual

## Getting started

Use it: open the **[app](https://AstraRocket.github.io/simulator/)**. It is the current release build, deployed to GitHub Pages.

To run it locally or build from source, see the **[AstraRocketSim README](https://github.com/AstraRocket/simulator#readme)**.

## Contributing

Code, bug reports, feature ideas, translations, and documentation are all welcome. See the **[AstraRocketSim CONTRIBUTING.md](https://github.com/AstraRocket/simulator/blob/master/CONTRIBUTING.md)** for how to get involved.

Everyone participating in this organization is expected to follow the **[Code of Conduct](https://github.com/AstraRocket/simulator/blob/master/CODE_OF_CONDUCT.md)**.

## License and attribution

All projects in this organization are released under the **GNU General Public License v3.0**.

The simulation engine derives from the [OpenRocket](https://openrocket.info/) core. The opt-in RASAero supersonic aerodynamics extensions are the original work of the mmrocket-sim project. Full credits and license lineage are in the individual repositories.

AstraRocketSim is an independent project and is not affiliated with or endorsed by the OpenRocket project, the National Association of Rocketry, or the Tripoli Rocketry Association.

## Safety and disclaimer

A simulation is a model, and a model is only as good as what it knows. Before you fly a rocket you designed here, read the **[Safety](https://AstraRocket.github.io/simulator/docs/safety)** page and check the rocket you actually built against it.

This software is provided "as is", without warranty of any kind, express or implied, including any warranty of accuracy, merchantability, or fitness for a particular purpose. Simulation results are estimates. They are not a substitute for the applicable safety code, a range safety officer, an airspace waiver, or your own judgment.

**You, and you alone, are responsible for any rocket you build, any motor you use, and any flight you make.** Neither AstraRocketSim, its contributors, nor the authors of the software it derives from accept any liability for injury, death, property damage, regulatory violations, or any other loss arising from use of this software or reliance on its output, to the fullest extent permitted by law. By using the software you accept this.

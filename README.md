# GOW Camera Packs

Free camera sets for iRacing, built for the [Global Open Wheel](https://globalopenwheel.com)
league's race broadcasts and shared for anyone to use: on your own streams, your
league's broadcasts, your replays. Licensed [CC BY 4.0](LICENSE): use them, change
them, put them on air; just credit GOW.

| | | |
|---|---|---|
| ![GOW TV](previews/mexicocity/gow-tv.jpg) GOW TV | ![Gopher cam](previews/mexicocity/gopher-2695.jpg) Gopher cam | ![Gopher cam, overhead](previews/mexicocity/gopher-1338-overhead.jpg) ...and the car goes over it |
| ![Wall cam](previews/mexicocity/wall-cam.jpg) Wall cam | ![Face cam](previews/mexicocity/face-cam.jpg) Face cam | ![Front low](previews/mexicocity/front-low.jpg) Front low |
| ![Drone](previews/mexicocity/drone.jpg) Drone | ![Low chase](previews/mexicocity/low-chase.jpg) Low chase | ![Shoulder cam](previews/mexicocity/shoulder-cam.jpg) Shoulder cam |

## What's in a pack

**Track files** (`cameras/tracks/<track>/<config>/gow.cam`) hold iRacing's own cameras,
untouched, plus our groups:

- **GOW TV**: our own trackside set. Tracking cameras placed from a driver's real laps,
  every position checked from replays so no tree, fence or grandstand gets between the
  lens and the car, and handed from one to the next all the way round the lap. Where a
  track has the spots for them it also has **gopher cams** (a lens in the road on the
  racing line, the car drives straight over it) and **wall cams** (low on a wall the
  cars run close to).
- **GOW Low Chase**: low behind the car.
- **GOW Front Low**: low in front, looking back as the car charges at the lens.
- **GOW Drone**: high behind, following.

**Car files** (`cameras/cars/<car>/gow.cam`) are optional and per car, for every track.
The sim gives a car nine fixed camera slots, so ours re-mount two of them and leave the
rest stock.

## Tracks

| Track | Config | Folder | What's ours | Updated |
|---|---|---|---|---|
| Autódromo Hermanos Rodríguez (Mexico City) | Grand Prix Historic | `mexicocity/gphistoric` | GOW TV (18 cameras, with gophers at 1338, 2040 and 2695 m and a wall cam at the Peraltada turn-in), GOW Low Chase, GOW Front Low, GOW Drone | 2026-10-08 |
| Autódromo José Carlos Pace (Interlagos) | Grand Prix | `interlagos/gp` | GOW TV (18 cameras, with gophers at 495 m, at the bottom of the drop from turn 1, and 3045 m, at the bottom of Mergulho, and wall cams at Descida do Lago and the Bico de Pato approach), GOW Low Chase, GOW Front Low, GOW Drone | 2026-10-12 |
| Miami International Autodrome | Grand Prix | `miami/gp` | GOW TV (25 cameras: 21 trackside, gophers at 1000 m, on the run to the esses, and in the turn 11 braking zone, and wall cams on the turn 1 and turn 17 approaches, where the cars brake within a metre or two of the barrier), GOW Low Chase, GOW Front Low, GOW Drone | 2026-10-22 |

Interlagos:

| | | |
|---|---|---|
| ![GOW TV](previews/interlagos/gow-tv.jpg) GOW TV | ![Gopher cam, turn 2](previews/interlagos/gopher-turn2.jpg) Gopher cam at the bottom of the turn 1 drop | ![Gopher cam, turn 2](previews/interlagos/gopher-turn2-over.jpg) ...and the car goes over it |
| ![Gopher cam, Mergulho](previews/interlagos/gopher-mergulho.jpg) Gopher cam at the bottom of Mergulho | ![Wall cam, Bico de Pato](previews/interlagos/wall-cam-bico-de-pato.jpg) Wall cam on the Bico de Pato approach | ![Wall cam, Descida do Lago](previews/interlagos/wall-cam-descida-do-lago.jpg) Wall cam at the Descida do Lago apex |

Miami:

| | | |
|---|---|---|
| ![GOW TV](previews/miami/gow-tv.jpg) GOW TV | ![Gopher cam, 1000 m](previews/miami/gopher-1000.jpg) Gopher cam on the run to the esses | ![Gopher cam, turn 11](previews/miami/gopher-turn11.jpg) Gopher cam in the turn 11 braking zone |
| ![Wall cam, turn 1](previews/miami/wall-cam-turn1.jpg) Wall cam on the turn 1 approach | ![Wall cam, turn 17](previews/miami/wall-cam-turn17.jpg) Wall cam on the turn 17 approach | |

## Cars

| Car | Folder | What's changed |
|---|---|---|
| Super Formula Lights | `superformulalights324` | **Nose** is a face cam (on the nose, looking back at the driver); **Gyro** is high over the driver's shoulder. Every other slot is stock. |

## Install

1. Download this repo (**Code > Download ZIP**) or clone it.
2. Copy its `cameras` folder into `Documents\iRacing\`, merging with what's there. Every
   file is called `gow.cam`, so nothing of yours is overwritten unless you already have a
   `gow.cam` in the same folder.
3. In the sim (a replay, or spectating), open the camera tool with **Ctrl+F12**, click
   **Load Track** (or **Load Car** for a car file), pick `gow.cam` and click **Open**.
4. Pick the GOW groups from the camera list. The sim remembers the last set you loaded
   for each track, so you only do this once.

The files are exported from the 2026 sim (track file version 18, car file version 15).
If an iRacing update changes the format, we'll re-export them here.

## Using them on air

For a director or automation: the group names are `GOW TV`, `GOW Low Chase`,
`GOW Front Low` and `GOW Drone`, and on the car `Nose` (face cam) and `Gyro` (shoulder).
Group numbers change when a set is loaded, so look groups up by name in the session's
`CameraInfo`, never by number. GOW TV hands the car from camera to camera by itself;
switch to it and leave it.

## Credit and licence

Our cameras are [CC BY 4.0](LICENSE). A credit line like this is plenty:

> Cameras: GOW Camera Packs by Global Open Wheel (github.com/ulchm/gow-camera-packs)

Each track file also carries iRacing's own stock cameras, which are iRacing.com's; the
licence covers what we added.

## About GOW

[Global Open Wheel](https://globalopenwheel.com) is an iRacing league racing Super
Formula Lights, with every round broadcast live. We're recruiting:
[globalopenwheel.com](https://globalopenwheel.com).

## Changelog

- **2026-10-22**: Miami (Grand Prix).
- **2026-10-12**: Interlagos (Grand Prix).
- **2026-10-08**: Mexico City (Grand Prix Historic) and the Super Formula Lights car file.

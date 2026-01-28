<div align="center">

# 15th MEU Shooting Range

**RFC / Product Requirements Document**

*A custom shooting range mod for training and qualification scenarios*

</div>

<br>

## Overview

A standardized shooting range with integrated scoring, timing, and performance tracking.  
Designed for training and qualification scenarios within the **15th MEU Realism Unit**.

<br>

## Features

### Targets
Standard Arma Reforger practice targets with hit registration and accurate scoring.

### Scoring
Per-player tracking throughout the session:

| Metric | Description |
|--------|-------------|
| Shots Fired | Total rounds discharged |
| Shots Hit | Successful target impacts |
| Shots Missed | Rounds that did not connect |

### Scoreboard
In-game display prop with real-time score updates and individual player performance.

### Timer
Configurable modes — countdown, count-up, or stopwatch — displayed above the scoreboard.

### Rangemaster Controls
| Action | Function |
|--------|----------|
| Pop Up | Raise all targets |
| Fold Down | Lower all targets |
| Configure | Timer settings |
| Clear | Reset scoreboard |

<br>

## Technical Architecture

| Component | Description |
|-----------|-------------|
| Target Entities | Vanilla targets with hit registration callbacks |
| Score Manager | Server-authoritative player stat tracking |
| Scoreboard Entity | Server-authoritative dynamic UI overlay (Screen) on a prop |
| Timer System | Server-authoritative, synchronized across all clients, displayed on the scoreboard |
| Rangemaster Interface | Tablet UI |

<br>

## Scope

**MVP (v0.1)**
- Single lane configuration (one player, one target)
- Two rangemaster controls (pop up/fold down)
- Scoreboard (no timer)


**Future**
- Leaderboards and historical records
- Qualification courses (pistol, rifle, etc.)
- CSV export

<br>

---

<div align="center">

*Developed for the [15th MEU Realism Unit](https://15thmeu.net/)*

</div>
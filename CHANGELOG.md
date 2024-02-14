# Changelog

All notable changes to this project will be documented in this file.

## [1.0.0-beta]

- Initial Release.

## [1.0.1-beta]

### Added

- Added RPM label.
- Added speed label(In Italian)

### Fixed

- Fixed janky looking PSI, Temps, and Grip Levels on tyres app.
- Removed extra digit from Estimated lap time from 00:00.000 to 00:00.00.
- Realigned a lot of elements. You shouldn't notice any shifting from screen to screen.

### Changed

- RPM changes color from green to red the higher the RPM.
- Reduced the precision on the PSI from 00.00 to 00.0 and reduced the update value to 1000ms.
- Took the edge off the 4 yellow shift indicators.
- Reduced the update time on Gap to Ahead, Behind and Gap to Leader to 1000ms.

### Removed

- Nothing

## [1.0.2-beta]

### Changed

- So I finally got the PSI down to 1 decimal place after realizing that it was a switch inside simhub keeping it at 2 places.
- Disabled steering input gauge until i figure out how to fix it.
- Optimised several update intervals. Wouldn't want your game to sacrifice FPS to process this Dashboard. :-)
- Swapped the Pit Service Screen for the Full Standings table screen. Pit Service Screen still available when you touch the Tyre/Gear widget on the right.
- Hid/Disabled features that dont yet work properly: Pit service widget. Lap timing widget.

### Fixed

- Fixed some typos in the changelog.
- Fixed the standings table on the Track Map Screen
- Fixed Relative Standings table.
- On the Pit Service Screen, changed pressure labels to PSI.
- Delta +/- Gauge was out of alignment by one pixel.
- Got the flags to work.

### ToDo

- Figure out how to fix/implement steering input.
- Pit Service Screen still optimized for iRacing. May fix it, or swap it out for something else.
- Optimise, then add more features.




## [1.0.3-beta]

### Added

- Brake temp indicators visible when dash detects ACC. AC has no brake temp data.
- Added heat color change to tyres and brakes according to Coach Dave Academy optimum temps in ACC.
- Added a Suspension Travel graphic to the tyres app(AC and ACC for now. Other sims calculate suspention compression differently so it till take time). Helpful when you record your session on simhub and replay it.

### Changed

- Started Optimizing for ACC.
- Fattened the tyred up a little bit. 
  
### Removed

- I could not find a metric for ACC Tyre wear in the telemetry data, so i scrapped it. (the % to be exact).

### Todo

- Figure out how to fix/implement steering input.
- Pit Service Screen still optimized for iRacing. May fix it, or swap it out for something else.
- Continue to optimize, then add more features.
- Implement the above on other sims. 

# [1.0.4-beta]


### Fixed

- Tweaked some wonky graphics here and there. 

### Added

- Re-implemented tyre wear. At first, I didn't understand how tyre wear worked in AC, and I found out it was actually grip level. So it would start out at somewhere around 97% then it would ramp up to 100% as the tyres heated up, and the grip level increased, then as you do more laps the grip level would then decrease until you need a tyre change. 

### Changed

- Changed the way tyres were represented graphically. I used linear gauges with the raw values instead of rectangles with complicated formulas. Simpler. I'm a simple guy. 


[1.0.0-beta]: https://github.com/lerontonge/Mission-Data-Dash-for-AC-ACC-AM2/releases/tag/v1.0.0-beta
[1.0.1-beta]: https://github.com/lerontonge/Mission-Data-Dash-for-AC-ACC-AM2/releases/tag/v1.0.1-beta
[1.0.2-beta]: https://github.com/lerontonge/Mission-Data-Dash-for-AC-ACC-AM2/releases/tag/v1.0.2-beta
[1.0.3-beta]: https://github.com/lerontonge/Mission-Data-Dash-for-AC-ACC-AM2/releases/tag/v1.0.3-beta
[1.0.4-beta]: https://github.com/lerontonge/Mission-Data-Dash-for-AC-ACC-AM2/releases/tag/v1.0.4-beta
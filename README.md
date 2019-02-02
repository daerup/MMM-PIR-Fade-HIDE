# MMM-PIR-Fade-HIDE

This is a Modul for the [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror). It is a modification of this Modul [mm-pir-hide-all](https://github.com/phrazelle/mm-pir-hide-all).
This modul adds a black Overlay with fading effect and do not deactivate the HDMI or graphical output!

## Dependencies

-   [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror)
-   [MMM-PIR-Sensor](https://github.com/paviro/MMM-PIR-Sensor)

## Installation

1. Clone this repo into `~/MagicMirror/modules` directory.
2. Configure your `~/MagicMirror/config/config.js`:

    ```
    {
			module: "MMM-PIR-Sensor",
			config: {
				sensorPin: 23,
				powerSaving: false,
			}
		},
		{
			module: "MMM-PIR-Fade-HIDE",
			position: "fullscreen_below",
			config: {
				fadeInTime: 3000,
				fadeOutTime: 3000,
				delay: 5000,
			}
		},
    ```

## Configuration Options

| **Option**         | **Default**                              | **Description**                         |
| ------------------ | ---------------------------------------- | --------------------------------------- |
| `fadeInTime`       | `1000`                                   | Time to fadeout     |
| `fadeOutTime`      | `1000`                                   | Time to fadein   |
| `delay`            | `5000`                                   | delay if the overlay is loading. Set to 0 for instant loading        |

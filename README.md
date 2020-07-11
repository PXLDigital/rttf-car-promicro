# rttf-car-promicro

## Pro Micro 5V 16Mhz


Change settings in file to adapt to your Receiver and Transmitter :

```c
// >>> Input signal modulation (uncomment only one!) <<<
#define PWM_RECEIVER  // Enable Pulse Width Modulation receiver
//#define PPM_RECEIVER  // Enable Pulse Position Modulation receiver

#define CHANNELS 3  // Override the default 6 channels (PPM max: 8, PWM max: 6)

// >>> Serial-Debug options for troubleshooting <<<
//#define SERIAL_DEBUG  // Enable Serial Debug by uncommenting this line
//#define SERIAL_SPD 115200  // Set debug bitrate between 9600-115200 bps (default: 9600)

// >>> Calibration settings <<<
#define CAL_CHANNEL 2  // Set which channel can trigger calibration on boot (default: 3 or 1)
//#define CAL_TIMEOUT 7000  // Custom delay in milliseconds to auto-accept calibration data (default: 5000)
//#define CAL_DISABLE  // Uncommenting this line causes the calibration to be disabled *
// (* when calibration disabled, do not forget to set stick center and halfway below!)
```
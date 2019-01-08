
[grbl + SuperPID2 = Super Awesome](http://www.eyemonline.com/?p=331)

`/grbl/config.h`

```h
// comment out
// #define DEFAULTS_GENERIC
// then add
#define DEFAULTS_SHAPEOKO_3


#define INVERT_SPINDLE_ENABLE_PIN // Default disabled. Uncomment to enable.
#define USE_SPINDLE_DIR_AS_ENABLE_PIN // Default disabled. Uncomment to enable.

// for grbl 0.9
#define SPINDLE_MAX_RPM 30000.0 // Max spindle RPM. This value is equal to 100% duty cycle on the PWM.
#define SPINDLE_MIN_RPM 0.0 // Min spindle RPM. This value is equal to (1/256) duty cycle on the PWM.

// for grbl 1.1
// comment out these to show defaults
//#define RPM_MAX  11686.4  // Max RPM of model. $30 > RPM_MAX will be limited to RPM_MAX.
//#define RPM_MIN  202.5    // Min RPM of model. $31 < RPM_MIN will be limited to RPM_MIN.
// set the max speed based on your router, these work for the Dewalt DWP611
#define RPM_MAX  30000  // Max RPM of model. $30 > RPM_MAX will be limited to RPM_MAX.
// set the min to 80, this seems to work well
#define RPM_MIN  80    // Min RPM of model. $31 < RPM_MIN will be limited to RPM_MIN.



// these are required for carbide motion v4
#define PARKING_ENABLE  // Default disabled. Uncomment to enable
#define ENABLE_PARKING_OVERRIDE_CONTROL   // Default disabled. Uncomment to enable
#define DEACTIVATE_PARKING_UPON_INIT // Default disabled. Uncomment to enable.


```

Pin 13 of the Arduino connects to the RUN input of SuperPID.

Add these changes into config.h, compile and load. Now M3 will start the spindle. 
M5 will stop the spindle. S commands will set the spindle speed.

Bridge the Z LIMIT terminals in order to allow updating your board.
KEEP IT BRIDGED WHILE UPDATING!!

[Compile and upload Grbl](https://github.com/gnea/grbl/wiki/Compiling-Grbl)

[Spindle Control](https://wiki.shapeoko.com/index.php/Shapeoko_3#Spindle_Control)



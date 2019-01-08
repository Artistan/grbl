#### [_Quick-Links:_](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration)

|  $   | config.h                        | Shapeoko XXL Defaults | Description                                                     |
| ---- |---------------------------------| --------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| $0   | DEFAULT_STEP_PULSE_MICROSECONDS | 10                    | [Step pulse, microseconds](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#0--step-pulse-microseconds)             |
| $1   | DEFAULT_STEPPER_IDLE_LOCK_TIME  | 255                   | [Step idle delay, milliseconds](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#1---step-idle-delay-milliseconds)  |
| $2   | DEFAULT_STEPPING_INVERT_MASK    | 0                     | [Step port invert, mask](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#2--step-port-invert-mask)                 |
| $3   | DEFAULT_DIRECTION_INVERT_MASK   | 6                     | [Direction port invert, mask](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#3--direction-port-invert-mask)       |
| $4   | DEFAULT_INVERT_ST_ENABLE        | 0                     | [Step enable invert, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#4---step-enable-invert-boolean)      |
| $5   | DEFAULT_INVERT_LIMIT_PINS       | 0                     | [Limit pins invert, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#5----limit-pins-invert-boolean)       |
| $6   | DEFAULT_INVERT_PROBE_PIN        | 0                     | [Probe pin invert, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#6----probe-pin-invert-boolean)         |
| $10  | DEFAULT_STATUS_REPORT_MASK      | 255                   | [Status report, mask](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#10---status-report-mask)                     |
| $11  | DEFAULT_JUNCTION_DEVIATION      | 0.02                  | [Junction deviation, mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#11---junction-deviation-mm)               |
| $12  | DEFAULT_ARC_TOLERANCE           | 0.01                  | [Arc tolerance, mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#12--arc-tolerance-mm)                          |
| $13  | DEFAULT_REPORT_INCHES           | 0                     | [Report inches, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#13---report-inches-boolean)               |
| $20  | DEFAULT_SOFT_LIMIT_ENABLE       | 0                     | [Soft limits, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#20---soft-limits-boolean)                   |
| $21  | DEFAULT_HARD_LIMIT_ENABLE       | 0                     | [Hard limits, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#21---hard-limits-boolean)                   |
| $22  | DEFAULT_HOMING_ENABLE           | 1                     | [Homing cycle, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#22---homing-cycle-boolean)                 |
| $23  | DEFAULT_HOMING_DIR_MASK         | 0                     | [Homing dir invert, mask](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#23---homing-dir-invert-mask)             |
| $24  | DEFAULT_HOMING_FEED_RATE        | 100                   | [Homing feed, mm/min](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#24---homing-feed-mmmin)                      |
| $25  | DEFAULT_HOMING_SEEK_RATE        | 2000                  | [Homing seek, mm/min](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#25---homing-seek-mmmin)                      |
| $26  | DEFAULT_HOMING_DEBOUNCE_DELAY   | 25                    | [Homing debounce, milliseconds](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#26---homing-debounce-milliseconds) |
| $27  | DEFAULT_HOMING_PULLOFF          | 5                     | [Homing pull-off, mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#27---homing-pull-off-mm)                     |
| $30  | DEFAULT_SPINDLE_RPM_MAX         | 30000                 | [Max spindle speed, RPM](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#30---max-spindle-speed-rpm)               |
| $31  | DEFAULT_SPINDLE_RPM_MIN         | 5000                  | [Min spindle speed, RPM](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#31---min-spindle-speed-rpm)               |
| $32  | DEFAULT_LASER_MODE              | 0                     | [Laser mode, boolean](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#32---laser-mode-boolean)                     |
| $100 | DEFAULT_X_STEPS_PER_MM          | 40.000                | [X steps/mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#100-101-and-102--xyz-stepsmm)                         |
| $101 | DEFAULT_Y_STEPS_PER_MM          | 40.000                | [Y steps/mmß](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#100-101-and-102--xyz-stepsmm)                        |
| $102 | DEFAULT_Z_STEPS_PER_MM          | 40.000                | [Z steps/mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#100-101-and-102--xyz-stepsmm)                         |
| $110 | DEFAULT_X_MAX_RATE              | 5000.000              | [X Max rate, mm/min](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#110-111-and-112--xyz-max-rate-mmmin)          |
| $111 | DEFAULT_Y_MAX_RATE              | 5000.000              | [Y Max rate, mm/min](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#110-111-and-112--xyz-max-rate-mmmin)          |
| $112 | DEFAULT_Z_MAX_RATE              | 5000.000              | [Z Max rate, mm/min](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#110-111-and-112--xyz-max-rate-mmmin)          |
| $120 | DEFAULT_X_ACCELERATION          | 400.000               | [X Acceleration, mm/sec^2](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#120-121-122--xyz-acceleration-mmsec2)   |
| $121 | DEFAULT_Y_ACCELERATION          | 400.000               | [Y Acceleration, mm/sec^2](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#120-121-122--xyz-acceleration-mmsec2)   |
| $122 | DEFAULT_Z_ACCELERATION          | 400.000               | [Z Acceleration, mm/sec^2](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#120-121-122--xyz-acceleration-mmsec2)   |
| $130 | DEFAULT_X_MAX_TRAVEL            | 845.000               | [X Max travel, mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#130-131-132--xyz-max-travel-mm)                 |
| $131 | DEFAULT_Y_MAX_TRAVEL            | 850.000               | [Y Max travel, mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#130-131-132--xyz-max-travel-mm)                 |
| $132 | DEFAULT_Z_MAX_TRAVEL            | 80.000                | [Z Max travel, mm](https://github.com/gnea/grbl/wiki/Grbl-v1.1-Configuration#130-131-132--xyz-max-travel-mm)                 |
         
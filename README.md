# IceWaddler2 Suite of Libraries

The IceWaddler2 FTC library suite, developed by FTC team #24135 Cybertronic PenguinZ over the past few years, contains the IceWaddler2 motion and pathing library, as well as supporting libraries to handle action-based opMode scheduling and gamepad inputs. These libraries are designed to be open, easily modifiable, and fundamentally simpler than alternative libraries. They are meant be modified internally, and to be customized to perform specific actions and achieve performance not possible with traditional, closed libraries. However, it's important to keep in mind that, due to the nature of these library, they are not as plug and play as other libraries, and requires a deeper understanding of the code rather that pure usage. Together, these libraries can handle auto pathing and actions, along with full teleops, including driver input, actions, and semiauto.

IceWaddler pathing is compatible with both mecanum and omni wheel drivetrains, and requires either a goBilda pinpoint computer or SparkFun OTOS for odometry. Motor encoder odometry may be added depending on demand.

We (FTC Team #24135) used IceWaddler2 (V2.1) for our auto pathing and action scheduling at Alberta Moose Meet 1. You can see IceWaddler in action in quals 6,9,12,14,and 18, at https://www.youtube.com/watch?v=fpYyWn9JR-o. (Our shooter was a bit inconsistent this meet, but I swear that the pathing was fine.)

All code is written by hand (No AI), mostly in a rush during before the start of the season, and thus is currently not very well commented or documented. Check out our team repo https://github.com/marcusxia-creator/FTC24135_BioBuzz/tree/MAIN_2026 for example code, and feel free to contact me on discord at ```dat_boi_in_space``` or email me at sylvanz20@gmail.com for more information about using IceWaddler.

## Installation
Copy (or merge if `lib` already exists) the `lib` package into the `./TeamCode/src/main/java/org/firstinspires/ftc/teamcode/` package. If you'd like to use the included and test auto `IWTestAuto.java` and odo offset calculator `OdoOffsetTester.java`(for goBilda pinpoint), you may also copy Your project should look like this:
~~~
/
├── libs/ (Ignore this package)
├── TeamCode/
│   ├── lib/ (Ignore this package)
│   └── src/
│       └── main/
│           ├── java/
│           │   └── org.firstinspires.ftc.teamcode/
│           │       ├── lib/
│           │       │   ├── CommandBase/
│           │       │   ├── GamepadDriver/
│           │       │   └── IceWaddler2/
│           │       ├── OpModes/
│           │       │   ├── IWTestAuto
│           │       │   └── OdoOffsetTester
│           │       ├── readme.md (The one that comes with the FTC SDK, not the one in this repo)
│           │       └── (The rest of your code also goes here)
│           └── res/
└── (The rest of the FTC SDK Contents)
~~~

## Usage
As mentioned earlier, documentation for this code is pretty sparse right now, and will be expanded later. For now, the best resource to figure out how to use IceWaddler2 is to read our code at https://github.com/marcusxia-creator/FTC24135_BioBuzz/tree/MAIN_2026, and start by copying our code structure. Tuning varies depending on how your hardware is configured, so, for now, just feel free to contact me at the contacts I mentioned earlier.

## License

Copyright (c) 2026 Sylvan Zheng
Distributed under the MIT License. See `LICENSE` for more information.
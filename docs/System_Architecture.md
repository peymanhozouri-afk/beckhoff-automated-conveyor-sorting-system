GVL_IO input mappings are intentionally disconnected.

VISU writes directly to GVL variables.

This preserves operator interface functionality.

# System Architecture

VISU
↓
GVL
↓
MAIN State Machine
↓
Function Blocks

FB_Conveyor
FB_Pusher
FB_ProductionTracker
FB_SpeedControl
FB_AlarmManager
↓
GVL Outputs
↓
GVL_IO

DO_ConveyorMotor
DO_RejectPusher
DO_GreenLight
DO_YellowLight
DO_RedLight
AO_VFDSpeedCmd
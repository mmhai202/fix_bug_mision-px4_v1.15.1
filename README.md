# Fix Bug in PX4 Mission Planning
- Issue Encountered:
  - After completing a mission flight, if the system is rebooted, subsequent missions are not executed.
- Solution:
  - Replace the mission_base.cpp file in the /src/modules/navigator directory of the PX4 v1.15.1 firmware.
  - To monitor mission progress, replace the MissionResult.msg file in the /msg directory of the PX4 v1.15.1 firmware, and observe the mission_has_been_activated and system_disarmed_while_inactive flags.

# MAVEn-Protocol
Protocol and Useful tips for MAVEn runs for ants &amp; fruit flies

USEFUL TIP
- thermocouple test 

![Picture1](https://user-images.githubusercontent.com/98350318/151409179-be4744b2-6027-4531-91f6-f3ea0746ad05.jpg)




Two main takeaways from placing thermocouples inside two of the chambers to measure the temperature of the air inside them while the whole thing was running. Started at 20C, then raised the temperature to 30C, then dropped it to 18C 
1) the chambers take about 20 minutes to reach the temperature set-point after making the change on the controller
2) the chambers on the edge are actually pretty close in temp to the ones in the middle, only 0.4 degrees C off when they were set to the high temp (30c) and only about 0.25 degrees C off when at the lower temperature (18c). 



Setting Up New Experimental Run

- Open gas cylinder
- Turn on LiCor 7000 (switch on front panel)
- Turn on MAVEn unit (switch on back panel)
- Note that steps 1-3 above should be done at least 1-3 hours prior to recording
- Verify that the USB cable from the MAVEn is connected to the labeled USB port on the laptop (left side, closest to the user).
- Open Maven_2 folder, select MAVEn programming, select MAVEn_A
- Turn on laptop and open the MAVEn_A.exe controller application
- On the Sign On panel, verify that it is connecting to the COM1 port and click “Sign On”
- Check the MAVEn Date and Time settings (may need adjusting depending on daylight savings time or time zone)
- Edit the recording settings:
- a. Dwell Time: how long it records from a channel (e.g. 120 s)
- b. Baseline Time: how long it records a baseline (e.g. 180 s)
- c. B/line Interleave ratio: how many channels it records from before repeating a baseline measurement (e.g. 16)
- d.Flow Rate Set mL/min: Gas flow rate (e.g. 25 mL/min)
- i. Note that with the FR, monitor channels for flow rates that may drop more than 20% as indicators of plumbing issues such as insufficient pressure, pinched tubing, etc.

- Click “Set MAVEn to Above Parameters” (if changing)
- Identify the Active Chambers (1-16); click Set Active Chambers
- Verify analog Inputs
- #1: CO2ppm (Transform 0 _ 30)
- #2: WVppt (Transform 0 _ 5)
- #3: RefBP (Transform 80 _ 8)
- #4: Volts4-Volts6 (not currently being used)
- Click the “Advanced/Diagnostic” tab at the top
- Click “Read Sensors” to verify light settings within an acceptable range
- Proceed to the “Run/Monitor” tab
- Click Monitor Data (1 Hz)
- Confirm flow rates and CO2 concentrations in expected ranges
- Click Stop Monitor
- Click “Spool to Text File, Using Comma Delimiter”
- Click Monitor Data (1 Hz)

ALL SET 👍

At this point, data are being recorded and saved every second. 

BUT WAIT 👀‼

Good time to verify that the laptop is either plugged in or has sufficient battery for however long the recording will last. 
With the settings above, a single run will take 35 minutes (2 minutes per chamber, 16 chambers, and a baseline) and it would be ideal to record at least 3-5 runs, so at 5 runs, that means just under 3 hours. That’s roughly enough time that the flies shouldn’t suffer any adverse effects (e.g. from isolation, food, water). 

# rss_HumanHand
This dataset consists of RSS data measured from smartphones carried by two human beings. Two users were required to stand at a certain distance from each other. In particular, distance = {0.2:0.2:2, 3:1:5}. For each distance, both smartphones will broadcast a BLE packet and also scan for the incoming packet for about 1min. The App is configured to log the following information: the truth distance, name of smartphone, MAC address of BLE chipset, the packet payload, RSS values, time elapsed, and timestamp. Two smartphones were used. The name of the smartphones is set to gryphonelab and HTC One M9, respectively.

# Consolidated Dataset
The smartphone also collected BLE packets from other BLE devices in the vicinity. Hence, we only consolidate the data from the two smartphones used in this experiment and exclude the BLE packets from other devices. Furthermore, we also apply a moving average filter to obtain a much smoother RSS value. The timestamp, packet payload and MAC address are discarded as some of them contain sensitive information while other might not convey meaningful information. The final consolidated dataset consists of the following information:
•	device name,
•	time elapsed,
•	rss (raw RSS value),
•	mRSS10 (filtered RSS value with window size = 10),
•	mRSS100 (filtered RSS value with window size = 100),
•	distance, and
•	label
** You can find this in the first raw.




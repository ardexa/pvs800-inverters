

## Documents
A. EN_PVS800_Central Inverter_FW_D_A4.pdf ... page 51


## Modbus Map
- Command: modpoll -a 1 -r 104 -c 10 -1 -p 503 192.168.1.1

Register		Name					Units		Notes
104			AC Voltage 1 		V
105			AC Voltage 2 		V
106			AC Voltage 3 		V
107			AC Current 1 		A
108			AC Current 2 		A
109			AC Current 3 		A
110			AC Power				W 		(multiply by 100)
112			Grid Freq			Hz 	(div by 100)
113			Cos Phi						(div by 100)


- Command: modpoll -a 1 -r 118 -c 12 -1 -p 503 192.168.1.1
Register		Name				Units	Notes
118 			DC Current		A
119 			DC Power			W		(mult by 1000)
120			Temperature		C
121			Status					convert by Dict
122			Fault						0 = No faults ; 1 = Fault active
123			Alarm						0 = No alarms ; 1 = Alarm active
127			Energy (kWh)
128			Energy (MWh)
129			Total Energy (GWh)
** Total Energy 	= GWh * 1000000 + MWh * 1000 + kWh
		

- Command: modpoll -a 1 -r 301 -c 16 -1 -p 503 192.168.1.1
Register		Name				Units	Notes
301 			DC Current 1	A		(div by 10)
302 			DC Current 2	A		(div by 10)
303 			DC Current 3	A		(div by 10)
304 			DC Current 4	A		(div by 10)
305 			DC Current 5	A		(div by 10)
306 			DC Current 6	A		(div by 10)
307 			DC Current 7	A		(div by 10)
308 			DC Current 8	A		(div by 10)
309 			DC Current 9	A		(div by 10)
310 			DC Current 10	A		(div by 10)
311 			DC Current 11	A		(div by 10)
312 			DC Current 12	A		(div by 10)
313 			DC Current 13	A		(div by 10)
314 			DC Current 14	A		(div by 10)
315 			DC Current 15	A		(div by 10)
316 			DC Current 16	A		(div by 10)



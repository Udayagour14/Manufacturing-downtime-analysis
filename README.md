# Manufacturing-downtime-analysis
Productivity &amp; downtime analysis for a soda bottling production line.
### calculate the efficiency for a production line and break it down by operator.
Create a new "Batch time" column in the "Line Productivity" tab that calculates the minutes between the "Start time" and "End time".
Create another new "Min batch time" column by looking up the value from the "Products" tab.
Date	Product	Batch	Operator	Start Time	End Time	Batch Time(minutes)	min batch time
2024-08-29	OR-600	422111	Mac	11:50:00	14:05:00	135	60
2024-08-29	LE-600	422112	Mac	14:05:00	15:45:00	100	60
2024-08-29	LE-600	422113	Mac	15:45:00	17:35:00	110	60
2024-08-29	LE-600	422114	Mac	17:35:00	19:15:00	100	60
2024-08-29	LE-600	422115	Charlie	19:15:00	20:39:00	84	60
2024-08-29	LE-600	422116	Charlie	20:39:00	21:39:00	60	60
2024-08-29	LE-600	422117	Charlie	21:39:00	22:54:00	75	60
2024-08-30	CO-600	422118	Dee	04:05:00	06:05:00	120	60
2024-08-30	CO-600	422119	Dee	06:05:00	07:30:00	85	60
2024-08-30	CO-600	422120	Dee	07:30:00	09:22:00	112	60
2024-08-30	CO-600	422121	Dennis	09:22:00	10:37:00	75	60
2024-08-30	CO-600	422122	Dennis	10:37:00	12:02:00	85	60
2024-08-30	CO-600	422123	Dennis	12:02:00	14:15:00	133	60
2024-08-30	CO-600	422124	Dennis	14:15:00	15:55:00	100	60
2024-08-30	CO-600	422125	Charlie	15:55:00	17:15:00	80	60
2024-08-30	CO-600	422126	Charlie	17:15:00	18:59:00	104	60
2024-08-30	CO-600	422127	Charlie	18:59:00	20:22:00	83	60
2024-08-30	CO-600	422128	Charlie	20:22:00	22:14:00	112	60
2024-08-30	CO-600	422129	Charlie	22:14:00	23:29:00	75	60
2024-08-31	CO-600	422130	Dee	07:45:00	09:05:00	80	60
2024-08-31	CO-600	422131	Dee	09:05:00	10:35:00	90	60
2024-08-31	CO-600	422132	Dee	10:35:00	11:35:00	60	60
![image](https://github.com/user-attachments/assets/0e62cd2e-388f-408f-bfa3-f56bb3068a93)


Calculate the "Efficiency" (sum of "Min batch time" / sum of "Batch time") for each operator.
Row Labels	Efficiency percentage
Charlie	67%
Dee	64%
Dennis	63%
Mac	61%
Grand Total	64%
![image](https://github.com/user-attachments/assets/1fcef8ea-2c37-4e12-8e71-32bd31a5edf3)
### Visualize the data using a bar chart
![image](https://github.com/user-attachments/assets/88800933-22d2-4a7c-b3ee-e00f55406103)
*As i conclude that Overall efficiency is around 64% 
but Mac has less efficiency precentage that we should focus.
![image](https://github.com/user-attachments/assets/505233ec-72eb-4469-96f9-0547c19d76d8)
### Identify main downtime factors
Create a "Downtime" column in the "Downtime factors" tab that sums the downtime for each factor from the "Line downtime" tab.
Create a "Pareto" column that calculates the % running total of downtime for each factor.
Downtime	Pareto
332	24%
254	42%
225	58%
160	70%
145	80%
74	86%
57	90%
49	93%
42	96%
33	99%
17	100%
0	100%
![image](https://github.com/user-attachments/assets/85704888-0166-4f62-9519-ba4273f074df)

Use a Pareto chart to identify the main factors for downtime in the production line.
![image](https://github.com/user-attachments/assets/b5e06857-8081-42f1-95ca-caa0a141451a)
![image](https://github.com/user-attachments/assets/652fc623-10c9-49e8-b741-0d70374b7bd2)

### Calculate downtime by operator & factor
I have calculate the total downtime by operator for each of the main factors identified.
I have created the operators data's as the rows and the main downtime factors as the columns.
Created Operator" column to the "Line downtime tab" and look up the values for each batch.
Create a total downtime for each operator by factor.
	6	7	4	2	8
	Machine adjustment	Machine failure	Inventory shortage	Batch change	Batch coding error
Charlie	118	85	17	10	44
Dee	79	36	85	20	30
Dennis	120	88	43	0	24
Mac	15	45	80	130	47
![image](https://github.com/user-attachments/assets/c16f7260-9daf-4b29-88eb-a2d26c8a145e)

## Formatting to make a recommendation.
![image](https://github.com/user-attachments/assets/3f0f233a-ac39-4092-a55d-ee30b80e6f26)



# analysis_task

The datasets contain the measurement data of battery testing. 

Some of the manufacturer information that is needed for performing analysis :

Cell capacity : 2.3 Ah

Operational Temperature : 25°C

C-rate = Current(A) / Cell Capacity (Ah)

Dataset Variables:

Data_Point : S.No	

Test_Time(s): Time step (1s) 

Current(A): Charging / Discharging Current ( + Ve charge, -Ve :discharge)	

Capacity(Ah): CurrentIntegral (Current *time(hrs) (ah)	

Voltage(V) : Cell/Battery Voltage (Operational range: 2.9V - 4.2V)

Energy(Wh): Energy (Voltage * Capacity)	

Temperature(℃)	: --

Date_Time	: Timestamp

Cycle_Index : Cycle Count ( 1 charge + 1 discharge = 1 cycle) 


Tasks To Do: 
Create a jupyter notebook.

1. Import the 2 datasets and join them as one file.
2. Analyse each variable such as voltage, time, current, capacity, energy, cycle_Index
3. Perform the exploratory data analysis (EDA : Univariate, Bivariate etc) and clean the data.
4. Extract only charging phase related data. (Charge when current > 0)
5. Calculate the charge_capacity for every cycle . (Capacity(k+1) = Capacity(k) + Current(k+1) * (time(k+1) - time(k))/3600)
6. Create a new variable c-rate. (see formula above)
7. Perform visualizations (Charge capacity vs Voltage , Charge capacity vs Cycle count etc. )
8. Explain the influence of c-rate on the charge_capacity

9. Use ML methods like poly. regression to extrapolate the total Charge capacity w.r.t cycle count.for every c-rate.
10. You are free to select any methodology you feel suitable to perform data analysis and visualizations.
11. Write your thought process behind every step you followed briefly.
12. Create a branch and Commit your changes to that repository.

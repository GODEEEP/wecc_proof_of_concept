# wecc_proof_of_concept
This repository demonstrates the GODEEEP project's approach to projecting load, wind, and solar time series under 
climate change. We demonstrated the approach using two weather years: 2017 and 2018. The 2017 data contains a late 
summer heat wave (Aug 26-Sep 3) impacting California and the southwestern U.S. The 2018 weather year had a more 
traditional mid-summer heat wave (Jul 3-9) that impacted most of the WECC.

## Input Files
The input data needed to recreate this demonstration is stored in the [data](data/) directory.

## Output Files
Average load, wind and solar ratio data by BA is stored in the [data](data/) directory. These ratios were calculated 
by taking the load, wind, and solar time series with climate change included (i.e., 2058) and dividing those by the 
time series from the base year (i.e., 2018). For completeness we computed annual mean ratios, mean ratios by month, and 
mean ratios during the heat wave event. Because the wind and solar capacity factors occasionally have very small values 
that make calculating ratios risky we capped the wind and solar capacity ratios at a maximum value of 3 before 
computing the averages. Missing values in the output files (e.g., when there is not enough wind or solar deployed in a 
BA) are marked as -999.

## Summary Plots
Quick-look plots analyzing the data are stored in the [plots](plots/) directory.

## Results by Balancing Authority for 2017 Weather Year
>
| BA | Load Time Series | Solar Time Series | Wind Time Series |
| :-: | :-: | :-: | :-: |
| AZPS  | <img src="plots/2017/AZPS_Load.png" width="50">  | <img src="plots/2017/AZPS_Solar.png" width="50">  | <img src="plots/2017/AZPS_Wind.png" width="50">  |
| BPAT  | <img src="plots/2017/BPAT_Load.png" width="50">  | <img src="plots/2017/BPAT_Solar.png" width="50">  | <img src="plots/2017/BPAT_Wind.png" width="50">  |
| CISO  | <img src="plots/2017/CISO_Load.png" width="50">  | <img src="plots/2017/CISO_Solar.png" width="50">  | <img src="plots/2017/CISO_Wind.png" width="50">  |
| PNM  | <img src="plots/2017/PNM_Load.png" width="50">  | <img src="plots/2017/PNM_Solar.png" width="50">  | <img src="plots/2017/PNM_Wind.png" width="50">  |
| PSCO  | <img src="plots/2017/PSCO_Load.png" width="50">  | <img src="plots/2017/PSCO_Solar.png" width="50">  | <img src="plots/2017/PSCO_Wind.png" width="50">  |

## Results by Balancing Authority for 2018 Weather Year
>
| BA | Load Time Series | Solar Time Series | Wind Time Series |
| :-: | :-: | :-: | :-: |
| AZPS  | <img src="plots/2018/AZPS_Load.png" width="50">  | <img src="plots/2018/AZPS_Solar.png" width="50">  | <img src="plots/2018/AZPS_Wind.png" width="50">  |
| BPAT  | <img src="plots/2018/BPAT_Load.png" width="50">  | <img src="plots/2018/BPAT_Solar.png" width="50">  | <img src="plots/2018/BPAT_Wind.png" width="50">  |
| CISO  | <img src="plots/2018/CISO_Load.png" width="50">  | <img src="plots/2018/CISO_Solar.png" width="50">  | <img src="plots/2018/CISO_Wind.png" width="50">  |
| PNM  | <img src="plots/2018/PNM_Load.png" width="50">  | <img src="plots/2018/PNM_Solar.png" width="50">  | <img src="plots/2018/PNM_Wind.png" width="50">  |
| PSCO  | <img src="plots/2018/PSCO_Load.png" width="50">  | <img src="plots/2018/PSCO_Solar.png" width="50">  | <img src="plots/2018/PSCO_Wind.png" width="50">  |
# sweden

The latest data should be downloaded from:
 https://covid.ourworldindata.org/data/ecdc/new_deaths.csv
 
 Prediction is based on the curve fitting with 10th degree polinomial: np.polyfit(x[valid],y[valid],10).
 
 Blue line is the predicted curve using the last 245 days from Nov. 11 in 2020. Red line is that using the last 110 days from Nov.11 in 2020. Black line shows the number of daily deaths due to the covid-19 from Dec. 31 in 2019 to Nov.11 in 2020.
 
 <img src='sweden.png' height=400 width=600>
 
 
 sweden.tar was encrypted by: 
 
 tar cvf - swedendaily.py |openssl enc -e -aes256 -out sweden.tar
 
 In order to expand sweden.tar, use the following command:
 
 openssl enc -d -aes256 -in sweden.tar|tar xv
 
 Of course, you need a password!
 
 

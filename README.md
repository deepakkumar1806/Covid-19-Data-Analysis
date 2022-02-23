# Covid-19-Data-Analysis
From the Covid19 and Vaccination Datasets, I have analysed the spread of covid19 across different levels in the country and also I have analysed vaccination status of different literacy group, age group, gender,etc. and estimated the duration required for total vaccination in India.



Plugins-
Software: python3 jupyter notebook (.sh files run python3 jupyter notebooks)

Environments: conda,python


Dependencies-
Python Libraries: pandas, numpy, matplotlib,json,datetime

Note - All input files are present in data folder

Programs-

.sh files:

assign1.sh 
top level script that runs the entire assignment

neighbors-districts-modifier.sh
runs q1.ipynb as
jupyter nbconvert --to notebook --execute q1.ipynb

case-generator.sh
runs q2.ipynb as
jupyter nbconvert --to notebook --execute q2.ipynb

edge-generator.sh
runs q3.ipynb as
jupyter nbconvert --to notebook --execute q3.ipynb

peaks-generator.sh
runs q4.ipynb as
jupyter nbconvert --to notebook --execute q4.ipynb

vaccinated-count-generator.sh
runs q5.ipynb as
jupyter nbconvert --to notebook --execute q5.ipynb

vaccination-population-ratio-generator.sh
runs q6.ipynb as
jupyter nbconvert --to notebook --execute q6.ipynb

vaccine-type-ratio-generator.sh
runs q7.ipynb as
jupyter nbconvert --to notebook --execute q7.ipynb

vaccinated-ratio-generator.sh
runs q8.ipynb as
jupyter nbconvert --to notebook --execute q8.ipynb

complete-vaccination-generator.sh
runs q9.ipynb as
jupyter nbconvert --to notebook --execute q9.ipynb

Jupyter Notebook files:

q1.ipynb
Input: neighbor-districts.json, cowin_vaccine_data_districtwise.csv
Output: nieghbors-districts-modified.json

q2.ipynb
Input: neighbors-districts-modified.json
Output: edge-graph.csv 

q3.ipynb
Input: district.csv,nieghbors-districts-modified.json
Output: cases-week.csv, cases-month.csv, cases-overall.csv

q4.ipynb
Input: active-case-week.csv, active-case-month.csv
Output: district-peaks.csv, state-peaks.csv, overall-peaks.csv

q5.ipynb
Input: cowin_vaccine_data_districtwise.csv,nieghbors-districts-modified.json
Output: district-vaccinated-count-week.csv, district-vaccinated-count-month.csv, district-vaccinated-count-overall.csv,state-vaccinated-count-weeks.csv,state-vaccinated-count-month.csv,state-vaccinated-count-overall.csv

q6.ipynb
Input: census.csv,cowin_vaccine_data_districtwise.csv,neighbors-districts-modified.json
Output: district-vaccination-population-ratio.csv,state-vaccination-population-ratio.csv,overall-vaccination-population-ratio.csv

q7.ipynb
Input: cowin_vaccine_data_districtwise.csv,neighbors-districts-modified.json
Output: district-vaccine-type-ratio.csv,state-vaccine-type-ratio.csv,overall-vaccine-type-ratio.csv

q8.ipynb
Input: census.csv,cowin_vaccine_data_districtwise.csv,neighbors-districts-modified.json
Output: district-vaccinated-dose-ratio.csv,state-vaccinated-dose-ratio.csv,overall-vaccinated-dose-ratio.csv

q9.ipynb
Input: census.csv,cowin_vaccine_data_districtwise.csv,neighbors-districts-modified.json
Output: complete-vaccination.csv

How to use:
In order to run all programs sequentially, run the following command from the terminal-
bash assign1.sh 


# Pre-Registration of Rpr - Reproduction of Kang et al 2020 Rapidly measuring spatial accessibility of COVID-19 healthcare resources: a case study of Illinois, USA

Elise Chan, Alana Lutz

## Planned Modification: Speed Limits
The speed limit dataset used in the original study has two issues that impact the accuracy of the study:
1. Some roads have multiple speed limits assigned to them with differences over 30mph. 
2. Many roads have missing speed limmits, and these roads were assigned a default speed limit of 35mph.

Instead of assigning 35mph to all missing speed limits, I will use the osmnx.speed package to fill in missing data using the mean speed limits of the other roads of the same type (residential, aterial, etc). 

To visualize the impact this change has on the study, I will generate the 4 maps of accessibility measure for population at risk/Covid-19 patients and ICU beds/ventilator. I will compare these to the maps from the first reanalysis without adjusted speed limits to see how this change impacts the study.

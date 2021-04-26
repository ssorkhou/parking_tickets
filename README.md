# Toronto Parking Tickets [![Binder](https://notebooks.gesis.org/binder/badge_logo.svg)](https://notebooks.gesis.org/binder/v2/gh/ssorkhou/parking_tickets/HEAD?filepath=An_Analysis_of_Toronto_Parking_Tickets.ipynb)

In this project we analyze Toronto parking tickets issued from 2018 to 2020. The data was obtained via the City of Toronto's [Open Data Portal](https://open.toronto.ca/) and the precise source of the data is [here](https://open.toronto.ca/dataset/parking-tickets/). With millions of parking tickets to analyze, we learned quite a bit about parking tickets in Toronto, such as the most ticketed locations, ticketing trends throughout the year, and the effects of COVID-19 on parking tickets. Follow along interactively using the "launch binder" button above.

This repository contains the following files:
- An_Analysis_of_Toronto_Parking_Tickets.ipynb
    - This is the Jupyter notebook containing the bulk of the project and is where we walk through our exploration of the data. We start by downloading the data from the Open Data Portal and then cleaning it up before beginning our analysis. We investigate and visually depict several interesting trends in the data, finishing with a few heatmaps depicting the distribution of parking tickets throughout Toronto.
- parking-ticket-data-readme.xls
    - This is the readme file as provided by the Open Data Portal.
- post_geocode.csv
    - The data provided by the City of Toronto records the location of a parking ticket by stating either the address of the building closest to the infraction or the intersection closest to the vehicle. While useful in their own right, latitudinal and longitudinal coordinates would be more beneficial if we wish to overlay the data on a map of Toronto. For this we used QGIS and OpenStreetMap to geocode the addresses. The data returned by QGIS is found in post_geocode.csv.

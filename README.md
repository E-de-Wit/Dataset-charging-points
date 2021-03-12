# Fastned

This dataset contains all the charging stations Fastned has at the time of publishing.
The goal is to convert Fastned.xlsx data into OpenStreetMap via a manual check.

The dataset format is likely to change whenever Fastned is going to provide this dataset on their [website](https://fastnedcharging.com/).
Therefore there currently is no script to convert the .gpx file, this has been done in Excel.

## Data usage
The data is free to use as open data under the [OCPI protocol](https://evroaming.org/) (Open Charge Point Interface).

## OpenStreetMap tags

It takes some basic knowledge of Excel in order to change the data (relatively) quickly.
For the manual conversion of the source data the following tags have been used:

Default tags:
* x=6,181513
* y=51,939637

Manual added- / changed tags:

* amenity=charging_station
* authentication:app=yes
* authentication:membership_card=yes
* fee=yes
* motorcar=yes
* opening_hours=24/7
* source=Fastned (OCPI)
* source:date=18-2-2021
* website=https://fastnedcharging.com
* operator=Fastned
* name=Fastned Geulenkamp
* socket:type2=2
* socket:type2:output=22 kW; 43 kW
* socket:chademo=2
* socket:chademo:output=50 kW
* socket:type2_combo=2
* socket:type2_combo:output=50 kW

These are example values based on one of the charging stations, the values differ based on the source data.
The adresses have not been taken into account because they are too inconsistent with the BAG-data and survey information.
The capacity has not been taken into account because the amout of sockets is not the same as the amount of available places to park.

## Comparing datasets

It is very likely that many charging stations within OpenStreetMap have already been mapped by other contributors, so make sure you take care to avoid duplicates.
Always use personal judgement and node history in order to change / remove exisiting information.

This dataset is not meant to be imported all at once.

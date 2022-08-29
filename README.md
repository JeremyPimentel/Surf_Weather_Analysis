# Surf_Weather_Analysis

## Overview
- The purpose of this analysis is to ultilize sqlalchemy and python to analysis weather data for a potential client. This data will provide an understanding of the yearly weather for a potential surf store. 

## Results
3 key differences were found as:
- 1) The mean temperature for June and Dcemeber was 77.2 and 71.1 respectively. 
- 2) The standard deviation for average tempertaure for June and December was 2.62 and 3.42 degrees respectively. 
- 3) Lastly, the min and max recorded tempertaures for June and December was 71/83, and 60/78 respectively. 

## Summary 
- The above results show that although December isn't quite frigid, it is considerably less warm than in June, and has more variability in daily temperaure as shown by the increased standard deviation and the difference in min a max recorded temperatures. 

Two additional queries could be to retrieve precipitation data. 

This could look like the following:
June_precipitation = session.query(Measurement.prcp).\
                  filter(Measurement.date >= '2017-06-01).\
                  filter(Measurement.date <= '2017-06-31)

December_precipitation = session.query(Measurement.prcp).\
                  filter(Measurement.date >= '2016-12-01).\
                  filter(Measurement.date <= '2016-12-31)

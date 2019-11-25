# Occupancy prediction model

This repository are provided with time series data from motion sensors (in this case [passive infrared sensors](https://en.wikipedia.org/wiki/Passive_infrared_sensor)). These sensors can be installed in buildings to help determine occupancy of rooms or movement in corridors. The data from these devices can be used to turn lights on and off or to derive optimized heating or ventilation schedules. Judging from the readings, we might know that nobody is usually in the office at a certain time of day so we can turn of the ventilation at this time. 

In this case, sensors were installed in 7 different meeting rooms of an office building and recorded occupancy values in these rooms for two months (July and August 2016). The objective is to creating a *model* which can *predict occupancy for the next 24h after a given timestamp*. The input for the predictor are all sensor readings up to the given timestamp. The output is a value of 1 if we predict that the room will be occupied and 0 if we predict that it will not be occupied for each of the following 24 hours.



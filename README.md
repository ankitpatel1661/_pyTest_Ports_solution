# _pyTest_Ports
## analyse sailing data
please analyse some sailing data for a ship.

## Two files can be found in subfolder data
* 'data.csv' = data received from one of our ships during sailing // 4 columns: (utc_time / Latitude / Longitude / SpeedOverGround)
* 'ports.csv' = database with port names and port location // 4 columns: (Latitude / Longitude / PortName / UN_PortCode)

## Remark about the port database
each port is defined by a port name, as well as a position (lat/long). the port coordinate is a random point within a city, or the port nearby. When looking for port calls, please have in mind, that the exact port coordinate will never perfectly match any ships-position. to find out if a ship called one specific port, one can use a tolerance, of for example +/-0.5 for Latitude and Longitude (feel free to use a different method)

## How can a port call be defined
For the sake of simplicity a port call is defined by the fact that the ship is not moving for a given time period (to be defined by the user) and the distance to the next port is within aforementioned tolerance of +/- 0.5 lat & long.

## Questions
* **Q 1**: Is any data missing? Expected signal frequency is 3min? please provide proof of your result.
* **Q 2**: What ports have been called by the ship. please provide a list of unqiue ports of call.
* **Q 3**: What was the total sailing time (total time the ship was moving between ports and not stationary)?
* **Q 4**: What was the total distance sailed?
* **Q 5**: Plot the speed profile between 2 ports of your choice.
* **Q 6**: What was the total time the ship did spend in each port?
* **Q 7**: How often was each port called (pls differentiate between unique port calls!)?
* **Q 8**: What was the highest average speed done between two ports?
* **Q 9**: Can you pls. create few interesting statistics/graphs of your choice about speed/distance/sailing time etc ... pls provide some interesting visuals about the dataset. 
* **Q 10**: What was the longest/shortest port call?
* **Q 11**: Can you create few interesting statistics/graphs of your choice about the port calls.
* **Q 12**: Can you compute the distance between two ports, using Latitude and Longitude data?
* **Q 13**: power demand for the ship as function of speed can be represented with this equation f(v) = +6.874*v^3 -83.274211*v^2 +659.5*v +9010.0 ... can you compute the total energy consumed for the sailing time?

* **Bonus 1**: Can you compare the "SpeedOverGround" signal with a self-computed Speed-over-Ground based on Latitude & Longitude position. What do you think about the quality of the signal "SpeedOverGround" when comparing it with the self computed signal? Can you provide some statistics and elaborate about the signal quality.

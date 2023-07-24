# _pyTest_Ports
## analyse sailing data to find ports of call and compute some statistics
we have to find out what our ship did during sailing. there are various questions. please start with the mandatory-questions. if done, feel free to pick any question from the optional-questions

## Two files can be found in subfolder data
* 'data.csv' = data received from one of our ships during sailing // 4 columns: utc_time;Latitude;Longitude;SpeedOverGround
* 'ports.csv' = database with port names and port location // 4 columns: LAT;LONG;PortName;UN_PortCode

## Remark about the port database
each port is defined by a port name, as well as a position (lat/long). this port coordinate is a random point within a city, or the port nearby. When looking for port calls, please have in mind, that the port coordinate will never perfectly match any ships-position. to find out if a ship called one specific port, one can use a tolerance, of for example +/-0.5 for lat and long

## How can a port call be defined
A port call is defined by the fact that the ship is not moving for at least one hour and the distance to the next port is within aforementioned tolerance of +/- 0.5 lat & long.

## Questions
* **Q 1**: Is data missing? Expected signal frequency is 3min? please provide proof of your result.
* **Q 2**: What ports have been called by the ship. please provide a list of unqiue ports of call.
* **Q 3**: What was the total sailing time?
* **Q 4**: Plot the speed profile between 2 ports of your choice.
* **Q 5**: How much time did the ship spend in each port?
* **Q 6**: How often was each port called (count unique port calls)?
* **Q 7**: What was the highest average speed done between two ports?
* **Q 8**: What was the longest/shortest port call?
* **Q 9**: What was the total distance sailed?
* **Q 10**: Can you compute the distance between two ports, using Latitude and Longitude data?


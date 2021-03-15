# Instructions to predict solar radiation in Grasshopper using GH_CPython 
1. The Rhino software version used is 5 and has to be "run as administrator" while opening.
2. The data used for machine learning model training can be downloaded from this link:

3. The pretrained neural netwrok model can be run in GH_NN_integration.ipynb for the prediction tasks. 
4. The pretrained neural netwrok model can be run in GH_DT_integration.ipynb for the prediction tasks.
5. The inputs in grasshopper file can be given as a list under the variable name '_input' as per the example shown below.

_input = [   <br />
12.0, # --> Hours <br />
1, # --> Building Context 00 <br />
2, # --> Building Context 01  <br />
1, # --> Building Context 02 <br />
2, # --> Building Context 03  <br />
9.0, # --> Month  <br />
1, # --> Facade floor level <br />
0.0, # --> Orientation <br />
10.0, # --> Facade floor height <br />
[-60.6, -45.0, 3.6], # --> Coordinate: 1 <br />
[-60.6, -45.0, 2.8], # --> Coordinate: 2 <br />
[-60.6, -45.0, 2.0], # --> Coordinate: 3  <br />
[-60.6, -45.0, 1.2], # --> Coordinate: 4  <br />
[-60.6, -45.0, 0.4], # --> Coordinate: 5  <br />
[-59.8, -45.0, 3.6], # --> Coordinate: 6  <br />
[-59.8, -45.0, 2.8], # --> Coordinate: 7  <br />
[-59.8, -45.0, 2.0], # --> Coordinate: 8  <br />
[-59.8, -45.0, 1.2], # --> Coordinate: 9  <br />
[-59.8, -45.0, 0.4], # --> Coordinate: 10  <br />
[-59.0, -45.0, 3.6], # --> Coordinate: 11  <br />
[-59.0, -45.0, 2.8], # --> Coordinate: 12  <br />
[-59.0, -45.0, 2.0], # --> Coordinate: 13  <br />
[-59.0, -45.0, 1.2], # --> Coordinate: 14  <br />
[-59.0, -45.0, 0.4], # --> Coordinate: 15  <br />
[-58.2, -45.0, 3.6], # --> Coordinate: 16  <br />
[-58.2, -45.0, 2.8], # --> Coordinate: 17  <br />
[-58.2, -45.0, 2.0], # --> Coordinate: 18  <br />
[-58.2, -45.0, 1.2], # --> Coordinate: 19  <br />
[-58.2, -45.0, 0.4], # --> Coordinate: 20  <br />
[-57.4, -45.0, 3.6], # --> Coordinate: 21  <br />
[-57.4, -45.0, 2.8], # --> Coordinate: 22  <br />
[-57.4, -45.0, 2.0], # --> Coordinate: 23  <br />
[-57.4, -45.0, 1.2], # --> Coordinate: 24  <br />
[-57.4, -45.0, 0.4]  # --> Coordinate: 25  <br />
]  <br />
5. More number of prediction  cases can be added  by appending to the python list - '_input'  <br />
6. Decision tree model file can be downloaded from this link: 
https://cf-my.sharepoint.com/:f:/r/personal/alammara_cardiff_ac_uk/Documents/Prediction%20Models?csf=1&web=1&e=g8Uevw  <br />
7. Inside GH_CPython module, in line 62 the path to simulation data has to be given and in line 190, the path to the DT model file has to be given.


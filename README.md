# Engineering-Sprints-Project

## OPTIFY - AN OPTIMAL FINDING AGENT

As we all know, navigation is becoming the basic need in the present world.When we want to travel to an unknownplace, asking people for the directions is 
not reliable. There comes the Google maps, which makes navigation much easier by providing the shortest possible path. But, when it comes to indoor 
navigation, we cannot completely rely on Google maps as it doesn't provide precise direction. 
Most of the time, when Google maps are used for a smaller area(i.e, college) rerouting is done or wrong destination is reached. This creates 
ambiguity to the user and wastes time and energy. In the current scenario, it is difficult to find an optimal path inside any campus like a college, company or 
any other organization. Hence, it is much needed to provide an an agent or a system for indoor navigation. Optify is an optimal path finding agent. It is 
designed in the motive of providing guidance to the people who comes in for an admission, competition, workshop, conference, etc. This system provides the 
shortest route to reach the given destination from the current source location. It provides step wise direction guide to the user. It reduces confusion in routing and saves time.

During the start of every academic year, various educational institutionswitness an inflow of many passionate students willing to pursue their dreams.During 
admission processes and various events,very often students, parents and other visitors find it difficult to reach to their desired locations. 

Even if they reach their desired location somehow they have to go through a lot confusion to reach the correct place.They are often guided manually by other 
visitors, students or workerswhich might be misleading and incorrect.

To overcome this problem, we aim to design an agent where one canchoosetheircurrent location (source) and destination. On doing this, apath will be 
displayed on the map. This pathrepresents the optimal route that connects the source to the destination. 

## FLOW DIAGRAM OF THE  PROPOSED SYSTEM

![image](https://user-images.githubusercontent.com/82304027/203695254-71c4d5a2-b36e-43f3-a765-3c279ae6c10e.png)

## METHODOLOGY

# 1.CREATE A MAP AND CONVERT INTO TILES:
•Draw the map of the desired campus by including all the locations and all possible routes.
•Once, the map is created convert it into tiles using tiled tool.

![image](https://user-images.githubusercontent.com/82304027/203695391-678699a9-ab47-401b-bff4-4efef305e33a.png)

![image](https://user-images.githubusercontent.com/82304027/203695450-b8c47bc3-78f6-45db-b779-7c7fb9c6af3b.png)


# 2.CREATE A BINARY VERSION OF THE MAP AND EXPORT IT TO CSV FILE:

•The image of the map is converted into 0’s and 1’s.

•The binary version of the image is exported as a csv file for further processing.

![image](https://user-images.githubusercontent.com/82304027/203695560-5d5f6541-3674-4736-8303-5b7109a9d50a.png)

# 3.PROCESSING THE CSV FILE AS A DATA FRAME

•CSV file is converted into a data frame using pandas python framework.

•Converting data frame into a matrix with appropriate coordinates (rows and columns).

![image](https://user-images.githubusercontent.com/82304027/203695643-71584e2f-631b-4419-931a-95bb620e3fee.png)

# 4.GET SOURCE AND DESTINATION AS INPUT

•The current location of the user is taken as a source and the final location to be reached as the destination.

•The source and the destination are mapped to the appropriate coordinates in the matrix.

![image](https://user-images.githubusercontent.com/82304027/203695737-a2a24dc4-63d7-445f-addd-6b0cf67b6d9f.png)

# 5.CALCULATING OPTIMAL PATH AND DISPLAYING THE ROUTE

•The shortest path between the given source and destination is calculated using the A* algorithm.

•A* algorithm is a heuristic function-basedalgorithm for proper path planning. It calculates heuristic function's value at each node on the work area and 
involves the checking of too many adjacent nodes for finding the optimal solution with zero probability of collision.

•Path is represented in theform of coordinates and each coordinate corresponds to the pixels in the map.

•The optimal path is displayed in the image to the user in the form of connecting lines from the source to the destination.

![image](https://user-images.githubusercontent.com/82304027/203695865-032d484c-7077-478e-beaf-4aae4808f80f.png)





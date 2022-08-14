# A-Star Project
In this project the A* algorithm is implemented to find the shortest distance between two points on a map. This can be useful for a transit map or cities using their GPS coordinates for example. In this case two such examples are shown. A New York subway transit map where each station is assigned a name and vertex position value and a cities of India map where each city is assigned its GPS vertices. After each location is given a vertex value a map is created where each location is placed in a dictionary along with its neighbors (the cities or stations that connect to it) and their respective distances from the location. The A* algorithm implements the following steps to find the shortest distance between two locations. 
    
    1. Assign start vertex a distance of 0 in min heap
    2. Assign every other vertex a distance of infinity in min heap
    3. Remove the vertex with the minimum distance from the min heap and set it to the current vertex
    4. While min heap is not empty:
        for each current vertex:
            for each neighbor in neighbors:
            new distance = (distance to current vertex) + (edge weight of current vertex to neighbor)
            if new distance is less than its current distance:
                current distance = new distance

        return distances
 There is only one file for this project, it is written in Python. In the file there is an example of how the code output that shows how it works, effectively listing the suggested route between two vertices.        

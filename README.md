
Side
2
av 4
IS-211 Spring 2022 Mandatory Assignment III v2022-03-18
IS-211 Mandatory assignment III
Choose between tasks A and B, i.e. you should only solve one of the tasks.
A. Network management
Problem 1
In this exercise we will direct our attention towards a (fictous) Internet connection
provider. The first priority of the company is to build an infrastructure that will allow
the company to provide internet connection to every domestic and business location
in the area.
Write a program that uses the data in the table below, and finds the cheapest way of
connecting all locations. The output of the program shall be the connections that are
needed specified with their endpoints in brackets (e.g. [A B]), and the total cost of the
connections.
A B C D E F
A 0 10 5 9999 3 12
B 0 17 9 17 12
C 0 35 3 12
D 0 9999 12
E 0 12
F 0
The table shows the cost of establishing a connection between pairs of locations.
Locations can be connect to themselves at no cost. The lower half of the table is
ommitted, because the cost of a connection is the same in both directions.
Problem 2: Routing tables
One of the reason for the success of the TCP/IP internet, is the robustness of the
routing algorithm. The routing algorithm used in IP, is usually a variant of Dijkstra's
Algorithm. The routing algorithm described below is a gross simplification of the real
protocol:
Page 1 of 4
IS-211 Spring 2022 Mandatory Assignment III v2022-03-18
● Each node on the network runs Dijktra's algorithm once, to find the fastest
route from that node to all the other nodes.
● Then the nodes exchange routing tables with their neighbours.
● If a node finds that routing packets through the neigbour is faster than the
best route the node has found, it will update its routing table using data from
the neighbors routing table
The following data may be useful for testing (it's the same graph as the table in the
distance table above. The format is one edge per line. Each line contains the name
of the two endpoints, and the cost.
A B 10
A C 5
A E 3
A F 12
B C 17
B D 9
B E 17
B F 12
C D 35
C E 3
C F 12
D F 12
E F 12
B. Travelling Salesman Problem
Find the path with the less cost from Timisoara to Bucharest by using a classical
TSP (see Figure 1).
Find in litterature ((Laporte, 2010), (Helsgaun, 2000), (The Traveling Salesman
Problem and Heuristics, 2013)) two different methods for the implementation of TSP
and implement it for the given problem in a programming language (Java, for
example).
Design and run benchmarking tests for both methods, reflect on the results and
conclude.
Page 2 of 4
IS-211 Spring 2022 Mandatory Assignment III v2022-03-18
Figure 1. Copy from (Russell & Norvig, 2010)
Hand in
The link to the Github repository with the source code, the specified output from the
programs, and a short note explaining why you made choices you did.
Specified output from the programs and the note must be delivered in particular
Canvas assignment.
References
Helsgaun, K. (2000). An effective implementation of the Lin–Kernighan traveling
salesman heuristic. European Journal of Operational Research, 126(1), 106–130.
https://doi.org/10.1016/s0377-2217(99)00284-2
Laporte, G. (2010). A concise guide to the Traveling Salesman Problem. Journal of
the Operational Research Society, 61(1), 35–40. https://doi.org/10.1057/jors.2009.76
Page 3 of 4
IS-211 Spring 2022 Mandatory Assignment III v2022-03-18
Russell, S., & Norvig, P. (2010). Artificial intelligence : a modern approach (3rd ed.).
Pearson.
The Traveling Salesman Problem and Heuristics. (2013).
https://ocw.mit.edu/courses/sloan-school-of-management/15-053-optimization-metho
ds-in-management-science-spring-2013/lecture-notes/MIT15_053S13_lec17.pdf
Part A based on Even Larsen/2020
Part B Janis Gailis/2022
END.
Page 4 of 4

# Multi-objective-Routing-Path-Optimization
The study shows an efficient method for improving communication efficiency in vehicle networks by using three optimisation algorithms, namely Dijkstra's Algorithm, Ant Colony Algorithm and Genetic Algorithm tailored to the particular requirements of this situation.

Introduction
An essential prerequisite for contemporary car networks on motorways is reliable internet access. Cars serve as relay nodes, sending data packets to other vehicles before establishing a connection with a base station (BS). The optimization problem is to identify a routing method that minimises latency and maximises the end-to-end data transmission rate for every car.

Objective
Determine the optimal routing path for each car to a base station, maximizing the end-to-end data transmission rate and minimizing latency.

Constraints
Two base stations with the following coorindates (BS-1 at (-1, -1) and BS-2 at (56325, 9)).
Distance-based transmission rates: Transmission rate varies with distance, and no connection is established if the distance exceeds 6000 meters.
Latency as the sum of delays in the routing path: The latency of each link is 50 milliseconds.

Problem Statement
In the quickly developing field of vehicular networks, especially in highway settings, data communication efficiency and dependability are critical. This project aims to improve the quality of Internet access for automobiles on a motorway, addressing an important optimisation challenge in this context. To guarantee the best possible Internet connectivity, the main goal is to create an optimisation solution that determines each vehicle in the network's most effective routing path. Every car in the network has the ability to function as a relay node, sending data packets to other cars until they arrive at a base station (BS). The task at hand involves determining the best route for data packets to go from every car to a base station (BS) while maximising two crucial parameters: the end to end data transmission rate and the end-to-end latency.

Data Preperation
The dataset in use comprises the geographical coordinates of vehicles on a motorway. The ability to compute the distances between vehicles, which has an immediate effect on the latency and data transmission speeds in the vehicle network, makes these coordinates essential. The dataset serves as the foundation for our network model. With the help of the vehicle placements, we can simulate a realistic vehicular network in which every car functions as a node with the ability to send data to base stations or other nodes (cars).

Graph Representation
The vehicle network is conceptualized as a graph where each vehicle represents a node. The edges between these nodes signify the potential for data transmission, weighted by factors derived from the distance between vehicles and the consequent transmission rates.

Effectiveness of Algorithms
- The Genetic Algorithm showed its proficiency in investigating a wide variety of possibilities and gradually progressing towards extremely effective paths. It was especially skilled at managing the problem's multi-objective structure and striking a balance between latency and transmission rate trade-offs.

- By simulating ant foraging behaviour, the Ant Colony Algorithm demonstrated its robustness in identifying effective routing patterns. This nature-inspired method proved excellent at dynamically adjusting to the intricate network topology and finding effective routes that strike a compromise between low latency and high transmission rates.

- Dijkstra's Algorithm focused on the cumulative weight of each path, which took latency and transmission rate into account, to effectively identify the most efficient paths. It performed exceptionally well in instances where the network conditions were steady and well-defined.

Limitations and Challenges
- The Genetic Algorithm, while powerful in exploration, required careful tuning of parameters and a sufficient number of generations to converge on optimal solutions, which might be computationally intensive.

- The Ant Colony Algorithm, despite its effectiveness, faced challenges in computational intensity due to the need for multiple ants and generations to establish reliable pheromone trails. This process can be time-consuming and resource-intensive.

- Dijkstra's Algorithm, though efficient, was somewhat limited in its adaptability to rapidly changing network conditions, as it always sought the shortest path based on current weights without considering potential future network dynamics.

- The Genetic Algorithm and Ant Colony Algorithm resulted in better solutiions due to the different approaches in the fitness function accompanied with the standard mutation and crossover techniques over generations.

References
Goldberg, D. E. (2013) Genetic algorithms in search, optimization, and machine learning. New Delhi, India: Pearson.
Avinash Navlani, Fandango, A. and Idris, I., 2021. Python Data Analysis. Packt Publishing Ltd.
Yim, A., Chung, C. and Yu, A., 2018. Matplotlib for Python Developers: Effective techniques for data visualization with Python. Packt Publishing Ltd.
Fan, D. and Shi, P., 2010. Improvement of Dijkstra’s algorithm and its application in route planning [online]. IEEE Xplore. Available from: https://ieeexplore.ieee.org/abstract/document/5569452.
Wang, Y. and Cai, Z., 2012. Combining Multiobjective Optimization With Differential Evolution to Solve Constrained Optimization Problems. IEEE Transactions on Evolutionary Computation, 16 (1), 117–134.
Gopal Prasad Malakar, 2017. Tutorial : Introduction to Genetic Algorithm n application on Traveling Sales Man Problem (TSP). YouTube [online]. Available from: https://www.youtube.com/watch?v=3GAfjE_ChRI.
Auctux, 2021. Solve the Traveling salesman problem (Genetic Algorithm, Ant Colony Optimization). YouTube [online]. Available from: https://www.youtube.com/watch?v=Sk9QQUGMdY8.

his repository contains several sets of test instances for the Covering Tour Location Problem. These instances are based on well-known Location Routing Problem benchmark instances and are extended by information on customer positions and coverings. All baseline LRP instances can be found at https://claudio.contardo.org/datasets-source-code/
Each folder contains a separate readme file with additional information.


**1. Test instances**

Test instance names follow their original LRP instance nomenclature and are extended by the number of customers and the covering radius, i.e. the maximum euclidean distance between a customer and a facility such that a customer can be covered by the respective facility. For instance, 'r30x5a-1_150_14_v3' is based on the 'r30x5a-1' instance by Akca et al., and contains 150 customers which can be covered by all facilities that are at most 14 units away.

Each test instances consists of a total of five files:

*_general.csv: no. of available depots and facilities, vehicle capacity and count, cost type (usually euclidean), and lower and upper LP bounds
*_customers.csv: contains information on customers (Demand and position in the euclidean space)
*_facilities.csv: position and capacity of intermediary facilities
*_coverings.json: dictionary that maps customers to all facilities that can be used to cover the given customer
Furthermore, files '_cost.json' contain a preprocessed distance cost matrix between all pairs of facilities and/or depots. Files titled '_depots.json' that are located in parent folders, such as 'r30x5a-1_depots.csv' located in '/akca/r30x5a-1/' contain depot information originally used for the baseline LRP instances.


**2. Results**

File Results.zip contains extensive information on the results obtained by both heuristics and the exact approach proposed in https://arxiv.org/abs/2411.17510. For more
information, please see the readme file.

**3. Plots**

File Plots.zip contains visualizations of the solution processes of both proposed heuristics. For more information, please see the readme file.

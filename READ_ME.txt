########GRID INSTANCES IN THE PAPER
x_y_{a,b}
x is the number of grid layers each of 5x5 nodes
y is the level of commodities
{a,b} is the population level: 
for level 'a' take population of each commodity (see set K in file dat) and multiply it for 3;
for level 'b' multiply it for 4.


########HOW TO READ FILE .DAT
NbNodes=;
NbArcs=; nb arcs in the list Edges + nb of additional arcs added due to our specific problem's features. These arcs are simply loops at the source nodes of the commodities. Note that there is no corresponding arc entry in the list Edges.
NbComm=;
NbTimeInt =is fixed to 15. Then time horizon goes from 0 to 15;
MaxLenght= max value of an arc trave time;
V= {list of nodes};
K = {<source, destination, population>};
Edges= {<tail,head>} these are directed arcs of the graph 
Length=[array of trave times];
Capacity=[array of arc capacities]; the last entries of these array (see value 1000000000) are capacities related to loops at source nodes.

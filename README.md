# csci2275-assignment-8--graph-solved
**TO GET THIS SOLUTION VISIT:** [CSCI2275 Assignment 8- Graph Solved](https://www.ankitcodinghub.com/product/csci2275-csci-2270-ae-data-structures-assignment-8-graph-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119714&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI2275  Assignment 8- Graph Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Objectives

1. Applications of the Breadth First Traversal

Instructions

Write code to apply the Breadth First Traversal. To receive credit for your code, you will need to pass the necessary test cases. Use the following steps to test your code as you work on the assignment:

1. Open up your Linux terminal, navigate to the build directory of this assignment (e.g. cd build).

2. Run the cmake .. command.

3. Run the make command.

4. If there are no compilation errors, two executables will be generated within the build directory: run_app_1 and run_tests.

5. If you would like to run your program including your app implementation in the main function, execute run_app_1 from the terminal by typing ./run_app_1.

6. To run the grading tests, execute run_tests from the terminal by typing ./run_tests.

Overview

In this assignment, you will apply the BFT for finding the shortest path in an unweighted graph.

The graph will be implemented using the following struct:

“` struct vertex; struct adjVertex{ vertex *v; }; struct vertex{

string name; bool visited = false; int distance = 0; vector&lt;adjVertex&gt; adj;

}; “`

NOTE: You are welcome to use the main function to test your code. The code in main_1.cpp is not being graded for this assignment.

Class Specifications

The Graph class definition is provided in the file Graph.hpp. Do not modify this file! Fill in the TODO implementations in file Graph.cpp according to the following specifications.

The vertex struct definition contains the key value in name, boolean member visited for use with the BFT algorithm, distance for keeping track of the BFT shorest distance, and adj vector for the adjacency list.

void addVertex(string name); + Search the existing vertices for a key match with name. If vertex already exists, do not add duplicate and print: cout&lt;&lt;vertices[i]-&gt;name&lt;&lt;” found.”&lt;&lt;endl; + If key is not found in the existing list of vertices, add new vertex to the graph.

void addEdge(string v1, string v2); + Add an edge between vertices named v1 and v2. + If either vertex v1 or v2 does not exist, then do nothing.

void displayEdges(); + Display all the edges in the graph in the following format:

If we create a graph with the following structure.

“` graph.addVertex(â€œATLSâ€); graph.addVertex(â€œECâ€); graph.addVertex(â€œAEROâ€); graph.addEdge(â€œATLSâ€, â€œECâ€); graph.addEdge(â€œAEROâ€, â€œECâ€); “`

We print the edges in the following manner.

ATLS –&gt; EC EC –&gt; ATLS AERO AERO –&gt; EC

The order of vertices printed is the same as the order in which they were added to the graph. Similarly, the order of vertices to the right of –&gt; sign is the same as the order in which the corresponding edge was added to the graph. void breadthFirstTraverse(string sourceVertex); + Breadth first traversal from sourceVertex. Format for printing:

// for the source vertex in the graph cout&lt;&lt; “Starting vertex (root): ” &lt;&lt; vStart-&gt;name &lt;&lt; “-&gt; “; // for other vertex traversed from source vertex with distance cout &lt;&lt; n-&gt;adj[x].v-&gt;name &lt;&lt;“(“&lt;&lt; n-&gt;adj[x].v-&gt;distance

&lt;&lt;“)”&lt;&lt; ” “;

int findShortestPathBetweenBuildings(string source, string dest); + Find the shortest distance path between the given source vertex and destination vertex in the graph. + Use the previous pointer to keep track of the shortest path. + Print the vertices along the shortest path, from start to end. + If not path exists between the vertices, print “No path between source and destination buildings!”

If we consider the graph to comprise of the following edges :

ATLS -&gt; CHEM CHEM -&gt; EC EC -&gt; AERO If the source vertex is CHEM and destination vertex is AERO then the shortest path distance would be 2.

Order of function implementation

1. addVertex

2. addEdge and displayEdges

3. breadthFirstTraverse

4. findShortestPathBetweenBuildings

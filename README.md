# comp5112-assignment-2-pthread-solved
**TO GET THIS SOLUTION VISIT:** [COMP5112 Assignment 2-Pthread Solved](https://www.ankitcodinghub.com/product/comp5112-assignment-2-pthread-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91304&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP5112 Assignment 2-Pthread Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Assignment 2: Pthread Programming

Assignment Description

Graph structural clustering is a common data analysis task to cluster vertices by their edge connec- tions in the graph. SCAN (Structural Clustering Algorithm for Networks) [1] is such an algorithm that clusters vertices based on a structural similarity measure. The algorithm is efficient in both computation and memory.

Figure 1: Illustration of data structure.

In our implementation, a graph G = (V, E) is stored in a CSR structure as shown in Fig. 1: where one array Neighbors stores the neighbors of all vertices, and the other array Offsets stores the offset of each vertex into the Neighbors array.

Please note that: (1) The length of the array Offsets is |V | + 1), with the last element of this array points to the end of Neighbors. (2) Accordingly, the length of Neighbors is the number of edges plus 1 (|E| + 1).

The SCAN algorithm, shown in Algorithm 1, can be divided into two stages: (1) find pivot vertices using the structural similarity measure, (2) expand clusters starting from the pivot vertices in the depth-first order.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Assignment 2 COMP5112/MSBD5009, 2021 Spring

</div>
</div>
<div class="layoutArea">
<div class="column">
1 2

3 4 5

6

7 8 9

10 11 12 13

<pre>14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
</pre>
</div>
<div class="column">
Algorithm 1: The SCAN Algorithm

Input : a graph G = (V, E), the structural similarity threshold ε, and the minimal cluster size μ

Output: the total number of clusters in G, and the cluster ID of each vertex main()

read files and initialization

// Stage 1: find pivot vertices each of which has at least μ neighbors whose similarity with the vertex exceeds ε

foreach v ∈ V do

foreach w ∈ Neighbors(v) do

Γ(v) ← N eighbors(v) ∪ {v}, Γ(w) ← N eighbors(w) ∪ {w}

</div>
</div>
<div class="layoutArea">
<div class="column">
if similarity(v, w) ← √

</div>
<div class="column">
&gt; ε then

</div>
</div>
<div class="layoutArea">
<div class="column">
|Γ(v)∩Γ(w)|

</div>
</div>
<div class="layoutArea">
<div class="column">
|Γ(v)|×|Γ(w)| Neighborsε(v) ← Neighborsε(v) ∪ {w}

end end

if |Neighborsε(v)| &gt; μ then pivots[v] ← true

else end

<pre>   // Stage 2:  expand clusters from pivot vertices
</pre>
foreach v ∈ V do

if pivots[v] and !visited[v] then

visited[v] ← true

cluster_result[v] ← v expansion(v, v)

num_clusters ← num_clusters + 1

else end

output num_clusters and cluster_result expansion(v, label)

foreach w ∈ Neighborsε(v) do

if pivots[w] and !visited[w] then

visited[w] ← true cluster_result[w] ← label expansion(w, label)

end end

Input and output

In this assignment, you will implement a pthread version of the SCAN algorithm. In the assignment folder:

• clustering_sequential.cpp is the sequential version for your reference. You can check the clustering result and compare its running time.

• clustering.h provides some utility funictions.

• main.cpp contains the main function of the pthread version.

• clustering_pthread_skeleton.cpp is the code skeleton for your work. Your task is to complete the following function which returns the array cluster_result:

int *scan(float epsilon, int mu, int num_threads, int num_vs, int num_es, int *nbr_offs, int *nbrs);

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Assignment 2 COMP5112/MSBD5009, 2021 Spring

</div>
</div>
<div class="layoutArea">
<div class="column">
• The datasets and results folders contain the datasets and clustering results respectively. Here is the output of executing the algorithm on ./sequential ../../data/test1/1.txt 0.7

3:

Screen output:

Elapsed Time: 0.000016516 s Number of clusters: 2

Result file output (sequential.txt):

2

-1 -1 -1 -1 -1 -1 6 6 -1 -1 -1 -1 -1 13 -1 13 -1 -1

2 in the first line is the number of clusters. The second line 6 13 is the cluster IDs (-1 if not in any cluster) of all vertices in order. Please note that in the parallel setting, we set the cluster ID be the lowest vertex ID of the pivots in the cluster. Make sure your file output follows the same format.

</div>
</div>
</div>

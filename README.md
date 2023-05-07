Download Link: https://assignmentchef.com/product/solved-ics-problem-sheet-1
<br>
<table width="572">

 <tbody>

  <tr>

   <td width="462"></td>

   <td width="110"></td>

  </tr>

  <tr>

   <td width="462"><strong>Problem 1.1: </strong><em>minimum spanning trees</em></td>

   <td width="110"> </td>

  </tr>

 </tbody>

</table>

We have introduced Kruskal’s algorithm for constructing random spanning trees (maze solutions). Edges are selected randomly and added to the spanning tree as long as the nodes connected by the edges belong to different equivalence classes. The original algorithm solves a slightly more difficult problem: Given a graph <em>G </em>= (<em>V,N</em>) and a cost function <em>c </em>that indicates the cost of including the edge <em>e </em>∈ <em>N </em>in the spanning tree, calculate the spanning tree <em>S </em>= (<em>V,E</em>) such that <em>C </em>= <sup>P</sup><em><sub>e</sub></em><sub>∈<em>E </em></sub><em>c</em>(<em>e</em>) is minimal (also called a minimum spanning tree). Kruskal’s algorithm solves this problem by selecting in each step an edge that joins two equivalence classes and has the minimum cost of all edges still available.

You are given the graph <em>G </em>= (<em>V,N</em>) with

<em>V </em>= {<em>a,b,c,d,e,f</em>}

<em>N </em>= {(<em>a,b</em>)<em>,</em>(<em>a,e</em>)<em>,</em>(<em>a,f</em>)<em>,</em>(<em>b,c</em>)<em>,</em>(<em>b,f</em>)<em>,</em>(<em>c,d</em>)<em>,</em>(<em>c,f</em>)<em>,</em>(<em>d,e</em>)<em>,</em>(<em>d,f</em>)<em>,</em>(<em>e,f</em>)} and the cost function <em>c </em>defined by the following table:

edge <em>e</em>:      (<em>a,b</em>)      (<em>a,e</em>)       (<em>a,f</em>)       (<em>b,c</em>)       (<em>b,f</em>)       (<em>c,d</em>)       (<em>c,f</em>)       (<em>d,e</em>)       (<em>d,f</em>)        (<em>e,f</em>)

cost <em>c</em>(<em>e</em>):        10           9             8             7             6             5             4             3             2             1

Construct a minimal spanning tree <em>S</em>(<em>V,E</em>) using Kruskal’s algorithm. For each step, write down the set of equivalence classes <em>A </em>and the edges in <em>E</em>. What is the overall cost <em>C </em>of the resulting spanning tree? You start with:

<em>E </em>= {}                                                                                             initialization, <em>C </em>= 0

<em>A </em>= {{<em>a</em>}<em>,</em>{<em>b</em>}<em>,</em>{<em>c</em>}<em>,</em>{<em>d</em>}<em>,</em>{<em>e</em>}<em>,</em>{<em>f</em>}}

<em>E </em>= <em>…                                                                                              </em>step 1, <em>C </em>= <em>…</em>

<em>A </em>= <em>…</em>

<em>E </em>= <em>…                                                                                              </em>step 2, <em>C </em>= <em>…</em>

<em>A </em>= <em>…</em>

<em>…</em>

<strong>Problem 1.2: </strong><em>boyer moore algorithm                                                                               </em>

You have designed a simple robot that can turn left (L), turn right (R), move one step forward (F), and pause (P) for short time. The robot is programmed by a sequence of robot instructions. For example, the sequence FFLFLFRFRFFLFRF will direct the robot through the maze shown on the slides discussing maze generation algorithms. Using the Boyer Moore algorithm, we can determine whether a robot program contains certain movement sequences.

Let Σ = {<em>L,R,F,P</em>} be an alphabet and <em>t </em>∈ Σ<sup>∗ </sup>be a text of length <em>n </em>describing a program for the robot. Let <em>p </em>∈ Σ<sup>∗ </sup>be a pattern of length <em>m</em>. We are looking for the first occurrence of <em>p </em>in <em>t</em>.

Consider the text <em>t </em>= <em>FFLFLFRFRFFLFRF </em>and the pattern <em>p </em>= <em>FFLFR</em>.

<ol>

 <li>Execute the naive string search algorithm. Show all alignments and indicate comparisons performed by writing uppercase characters and comparisons skipped by writing lowercase characters. How many alignments are used? How many comparisons are done?</li>

 <li>Execute the Boyer-Moore string search algorithm with the bad character rule only. How many alignments are used? How many comparisons are done?</li>

 <li>Calculate the lookup table for the bad character rule that indicates the number of alignments that can be skipped if a comparison does not match.</li>

</ol>

<strong>Problem 1.3: </strong><em>big </em><em>O notation              </em>(1+1 = 2 points) a) Sort the functions

in increasing order concerning their big <em>O </em>membership. (It is sufficient to provide the correct order.)

<ol>

 <li>b) Given the functions <em>f,g,h </em>: N → N, show that the following transitivity property holds: If <em>f </em>∈ <em>O</em>(<em>g</em>) and <em>g </em>∈ <em>O</em>(<em>h</em>), then <em>f </em>∈ <em>O</em>(<em>h</em>).</li>

</ol>
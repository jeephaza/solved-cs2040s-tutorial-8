Download Link: https://assignmentchef.com/product/solved-cs2040s-tutorial-8
<br>
<h1>Problem 1.            DFS/BFS</h1>

Recall that when performing DFS or BFS, we may keep track of a parent pointer that indicates the very first time that a node was visited. Explain why these edges form a tree (i.e., why there are no cycles).

<h1>Problem 2.           Graph components</h1>

(Relevant Kattis Problem: https://open.kattis.com/problems/countingstars)

Given an undirected graph <em>G </em>= (<em>V,E</em>) as an adjacency list, give an algorithm to: (i) determine if the graph is connected; (ii) return the number of connected components (CC) in the graph.

<h1>Problem 3.             Good students, bad students</h1>

(Relevant Kattis problem: https://open.kattis.com/problems/amanda)

There are good students and bad students<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>. And at the end of every year, we have to divide the students into two piles: <em>G</em>, the good students who will get an A, and <em>B</em>, the bad students who will get an F. (We only give two grades in this class.)

To help with this process, your friendly tutors have each created a set of notecards. Each card contains the names of two students. One of the two names is a good student, and the other is a bad student. Unfortunately, they do not indicate which is which.

Since the notecards come from thirty eight different tutors, it is not immediately certain that the cards are consistent. Maybe one tutor thinks that Humperdink is a good student, while another tutor thinks that Humperdink is a bad student. (And Humperdink may appear on several different cards.) In addition, the tutors do not provide cards for every student.

Assume you can read the names on a card in <em>O</em>(1) time and that there are more good students than bad students.

Devise an algorithm to determine the answers for the following questions:

<ul>

 <li>Are the notecards are consistent, i.e., is there <em>any </em>way that we can assign students to <em>G </em>and <em>B </em>that is consistent with the cards?</li>

 <li>Are the notecards sufficient? i.e., is there one or more than one way of assigning students to the sets <em>G </em>and <em>B</em>?</li>

 <li>Assuming that the notecards are consistent and sufficient, determine which set each student belongs in.</li>

</ul>

<h1>Problem 4.           Word games</h1>

(Relevant Kattis problem: https://open.kattis.com/problems/sendmoremoney)

Consider the following two puzzles:

<ul>

 <li>Puzzle 1:</li>

</ul>

S E N D

+ M O R E

———-

M O N E Y

<ul>

 <li>Puzzle 2:</li>

</ul>

F O R T Y

T E N

+                T E N

————

S I X T Y

In each of these two puzzles, you can assign a digit (i.e., {0<em>,</em>1<em>,</em>2<em>,</em>3<em>,</em>4<em>,</em>5<em>,</em>6<em>,</em>7<em>,</em>8<em>,</em>9}) to each of the letters in the puzzle such that the given equation holds. (Each digit is only assigned to once letter.) The goal is to solve these puzzles. How should you model and solve these puzzles? What is the running time of your solution? Can you optimize your solution to find the answer more quickly, most of the time?

<strong>Problem 4.a. </strong>Explain how to model the problem as a graph search problem. What are the nodes? How many nodes are there? What are the edges? Where do you start? What are you looking for?

<strong>Problem 4.b. </strong>To solve this problem, should you use BFS or DFS? Why? How else can you make it run faster?

<strong>Problem 4.c.    </strong>When does your search finish? Can you optimize the algorithm to minimize the amount of searching?

<h1>Problem 5.           Graph modeling</h1>

(Relevant Kattis Problem: https://nus.kattis.com/sessions/qxixc8/problems/nus.cs3233mh)

Here are a bunch of problems. How would you model them as a graph? (Do not worry about solving the actual problem. Just think about how you would model it as a graph problem.) Invent some of your own problems that can be modeled as graph problems—the stranger, the better.

<strong>Problem 5.a. </strong>Imagine you have a population in which some few people are infected with this weird virus. For any two patients, you want to decide whether the infection might have spread from one to the other via some intermediate asymptomatic patients. You suspect that if such a path exists it isn’t too long (since most cases are not asymptomatic.)

<strong>Problem 5.b. </strong>Imagine you have a population in which some few people are infected with this weird virus. You also have a list of locations that each of the sick people were in during the last 14 days. Determine if any of the sick people ever met.

<strong>Problem 5.c. </strong>You are given a set of jobs to schedule. Each job <em>j </em>starts at some time <em>s<sub>j </sub></em>an ends at some time <em>t<sub>j</sub></em>. Many of these jobs overlap. You want to efficiently find large collections of non-overlapping jobs so that you can assign each collection to a single server.

<strong>Problem 5.d. </strong>An English professor complains that students in their class are cheating. The professor suspects that the cheating students are all copying their material from only a few different sources, but does not know where they are copying from. Students that are not cheating, on the other hand, all submit fairly different solutions. How should we catch the cheaters?

<strong>Problem 5.e.    </strong>There are <em>n </em>children and <em>n </em>presents, and each child has told you which presents they want. How do we assign presents to children?

<h1>Problem 6.            A problem lovely as a tree</h1>

(Relevant Kattis Problem: https://open.kattis.com/problems/flyingsafely)

Assume you are given a connected graph with <em>n </em>nodes and <em>m </em>edges as an adjacency list. (You

are given <em>n </em>but not <em>m</em>; assume each adjacency list is given as a linked list, so you do not have access to its size.)

Give an algorithm to determine whether or not this graph is a <em>tree</em>. Recall that a tree is a connected graph with no cycles. (What if you want to find a cycle?)

Your algorithm should run in <em>O</em>(<em>n</em>); particularly, it should be independent of <em>m</em>. Assume <em>O</em>(<em>n </em>+ <em>m</em>) is too slow.

<h1>Problem 7.           Gone viral</h1>

There are <em>n </em>students in the National University of Singapore. Among them, there are <em>n </em>− 1 friendships. Note that friendship is a symmetric relation, but it is not necessarily transitive.

Any two people in the National University of Singapore are either directly or indirectly friends. Formally, between any two different people <em>x </em>and <em>y</em>, either <em>x </em>is friends with <em>y </em>or there exists a sequence <em>q</em><sub>1</sub><em>,q</em><sub>2</sub><em>,…,q<sub>k </sub></em>such that <em>x </em>is friends with <em>q</em><sub>1</sub>, <em>q<sub>i </sub></em>is friends with <em>q<sub>i</sub></em><sub>+1 </sub>for all <em>i &lt; k </em>and <em>q<sub>k </sub></em>is friends with <em>y</em>.

It was discovered today that <strong>two </strong>people were found to have the flu in the National University of Singapore.

<strong>Figure 1: </strong><em>Gone Viral. </em>(Matthew Ng Zhen Rui)

Every day, every person can meet with <strong>at most one friend. </strong>When these two people meet, if exactly one of them has the flu, it will be transmitted to the other.

Give an <em>O</em>(<em>n</em>log<sup>2 </sup><em>n</em>) algorithm to determine the minimum possible number of days before it is possible that <em>everyone </em>has the flu.

Hint: First, solve the case where there is only a single person was infected at the start in

<em>O</em>(<em>n</em>log<em>n</em>)

<a href="#_ftnref1" name="_ftn1">[1]</a> No, not really. This sort of binary distinction is silly.
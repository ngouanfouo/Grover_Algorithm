# Grover-s-Algorithm-for-Graph-Colouring

---

## **Introduction** 
This project extends your work in Week 18 to use Grover's algorithm for more advanced problems known as Graph Coloring Problems. You will learn how to build your own an oracle and solve several types of problems that can all be reduced to Graph Coloring.

<br>

## **Description**
In Computer Science, Graph Coloring is one of many so-called "graph problems". Although the mathematical representation and analysis of these problems can get very complex, graph coloring is actually pretty simple. **We can view graph coloring as trying to answer the question, "Can we color every country on a map without any touching countries having the same color, given *k* colors?"**

<br>

It turns out that this problem is extremely powerful and can be used to represent many other problems including:
* Sudoku (numbers instead of colors in a 9X9 map)
* Scheduling
* Networking
* Machine Learning (ex: clustering)

Therefore, solving such a problem is very important!

<br>

We will see how to use Grover's algorithm for this problem, particularly learning how to use Grover to search of a *list of solutions* instead of through a literal databse. This is actually believed to be the more likely use of Grover once we have fault tolerant computers, due to the difficulty of encoding databases into quantum states in part.

We will follow these steps for building and solving a problem with Grover:
1. Create an initial state preparation circuit. This will put all possible solutions in equal superposition.
1. Create an oracle circuit. This will flip the phase of correct solutions and leave the rest alone. Defining this is often the hardest part.
1. Define the problem using Qiskit's `Amplification(...)` function.
1. Solve the problem using Qiskit's `Grover(...)` function. We usually have to run several times with different number of iterations to get a good result.



**NOTE**: This project will involve looking at many histograms of results. As the size of the problems increase, so will the number of solutions we see in our graphs. If you start having trouble seeing the individual bars and states in the graphs, you can click on them to zoom in OR right click and press "Save Image As..." to download onto your computer and open it up in a larger window.

<br>

## **Key Questions**
In this project, you will answer the following questions:
1. When using Grover's algorithm, we do not get good results for too few *or* too many iterations. Rather, there is a "sweet spot" (a balanced number of iterations) right in the middle. Why is this?
2. How and why does having *multiple* correct answers change the number of iterations needed for Grover's algorithm?
3. The best classical algorithm that guarantees solutions to the 4 coloring problem has a Big-O complexity of $O(1.7272^n)$ where $n$ is the number of Countries to be colored (or Routes to be assigned planes). How does Grover's algorithm compare to this run time?

<br>

## **Structure**
This project is broken into 2 parts:
> **Part 1**: Grover for 2 Coloring Problems
>
>> **Part 1.1**: Building a Specific Problem
>>
>> **Part 1.2**: Building General Problems
>>
>> **Part 1.3**: Solving General Problems
>
> **Part 2**: Grover for 4 Coloring Problems
>
>> **Part 2.1**: A First Approach
>>
>> **Part 2.2**: A Faster Approach
>>
>> **Part 2.3**: Beyond Coloring
>
> **Wrapping Up**

<br>

## **Resources**

* [Week 18 Lab Solutions (Grover's Algorithm for Searching Databases)](https://drive.google.com/file/d/1BAYHXCpXLp-iP2WyvamVbRchshwxOquM/view?usp=sharing)
* [Qiskit Textbook: Grover for Sudoku](https://qiskit.org/textbook/ch-algorithms/grover.html#sudoku)
* [Qiskit Documentation: Grover’s Algorithm and Amplitude Amplification](https://qiskit.org/documentation/tutorials/algorithms/06_grover.html)
* [Qiskit Documentation: `AmplificationProblem(...)`](https://qiskit.org/documentation/stubs/qiskit.algorithms.AmplificationProblem.html)
* [Qiskit Documentation: `Grover(...)`](https://qiskit.org/documentation/stubs/qiskit.algorithms.Grover.html)
* [Qiskit Documentation: `circuit.mct(...)`](https://qiskit.org/documentation/stubs/qiskit.circuit.QuantumCircuit.mct.html)

**If you're curious to learn more:**
* [Youtube: The Four Color Theorem - What Counts as a Proof?](https://www.youtube.com/watch?v=42-ws3bkrKM)

---

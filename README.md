# SBST22 Tutorial

This is the repository for the [SBST 2022 tutorial](https://sbst22.github.io/keynotes/) on "Learning and Refining Input Grammars for Effective Fuzzing".

## Prerequisites

- Download [Python 3.10](https://www.python.org/downloads/)
   
  Some variation of
  ```
  $ sudo apt-get install python3.10
  ```
- Install [Jupyter](https://jupyter.org/).
  ```
  $ pytho3 -m pip3 install jupyter
  ```
- Install [Graphviz](https://graphviz.org/download/) for your operating system.
  
  Some variation of
  ```
  $ sudo apt install graphviz
  ```
- Checkout this repository
  ```
  git clone git@github.com:vrthra/SBST22-tutorial.git
  ```
- Start the Jupyter server in the repository directory
  ```
  $ cd SBST22-tutorial
  $ jupyter-notebook
  ```
  This opens a browser window at http://localhost:8888/tree
- Proceed to [x0_0_Prerequisites.ipynb](http://localhost:8888/notebooks/x0_0_Prerequisites.ipynb) and execute the page completely.

## Stepping through the tutorial

The jupyter notebooks in this tutorial are designed to be stepped through in an ordered sequence.
For example, The first number `0` in `x0_3_HDD.ipynb` is the major number and `3` is the minor number.
The major number describes the particular section being explained. These are:

0. Prerequisites

   These are well known external algorithms, and will not be explained during the tutorial.
1. Generating Samples

   How to generate valid samples for grammar mining when one does not have access to the input specification for parsers (e.g. JSON, Java syntax etc.).
   
2. Mining Grammar

   How to mine the context-free grammar of a given parser
   
3. Abstracting Inputs

   If you find a bug or an otherwise interesting behavior, how to abstract this input so that you can generate a much larger number of inputs all reproducing this behavior.
   
4. Input Algebras

   If you find multiple such interesting beahviors, or bugs, how to combine them, using the full algebraic operations -- conjunction (and), disjunction (or), and negation (complement) so that each input contains all bugs you specify.

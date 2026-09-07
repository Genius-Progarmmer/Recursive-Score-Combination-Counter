# Recursive Score Combination Counter

A C++ program that calculates the number of different ways to reach a target score using moves of 2 or 3 points.

## Overview

The program starts with a score of `0` and attempts to reach exactly `7`.

At every step, the program has two possible choices:

* Add 2 points
* Add 3 points

The program uses recursion to explore every possible sequence of choices.

## How It Works

The `play()` function receives the current score:

```cpp
void play(int score)
```

If the score reaches exactly `7`, the program counts that sequence as a valid way.

If the score becomes greater than `7`, that path is stopped.

Otherwise, the program explores both possible score increases:

```cpp
play(score + 2);
play(score + 3);
```

## Result

For a target score of `7`, the program outputs:

```text
Number of ways: 3
```

## Requirements

* C++ compiler
* Standard C++ library

## Compile

Using g++:

```bash
g++ main.cpp -o score_counter
```

## Run

```bash
./score_counter
```

On Windows:

```bash
score_counter.exe
```

## Concepts Demonstrated

* Recursion
* Base cases
* Path exploration
* Counting solutions
* Algorithmic problem solving
* C++ functions

## Project Structure

```text
Recursive-Score-Combination-Counter/
└── main.cpp
```

## Technologies

* C++
* Standard Library
* Recursion

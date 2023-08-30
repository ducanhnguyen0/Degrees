# Degrees: A "Six Degrees of Kevin Bacon" game AI

Harvard CS50AI Project

## Description:

A program using Breadth-First-Search algorithms to find the shortest path in order to detect "degrees of separation" apart two actors are.

## Tech Stack:

* Python

## Background:

According to the Six Degrees of Kevin Bacon game, anyone in the Hollywood film industry can be connected to Kevin Bacon within six steps, where each step consists of finding a film that two actors both starred in.

In this problem, we’re interested in finding the shortest path between any two actors by choosing a sequence of movies that connects them. For example, the shortest path between Jennifer Lawrence and Tom Hanks is 2: Jennifer Lawrence is connected to Kevin Bacon by both starring in “X-Men: First Class,” and Kevin Bacon is connected to Tom Hanks by both starring in “Apollo 13.”

We can frame this as a search problem: our states are people. Our actions are movies, which take us from one actor to another (it’s true that a movie could take us to multiple different actors, but that’s okay for this problem). Our initial state and goal state are defined by the two people we’re trying to connect. By using breadth-first search, we can find the shortest path from one actor to another.

## Project Specification:

### shortest_path
The function returns the shortest path from the person with id source to the person with the id target which is a list, where each list item is the next (movie_id, person_id) pair in the path from the source to the target. Each pair should be a tuple of two strings.

## How to run

1. Clone this project
2. Run command line in terminal:
   ```
   python degrees.py 'dataset file'
   ```
   (You can use either `small` or `large` for the dataset file)

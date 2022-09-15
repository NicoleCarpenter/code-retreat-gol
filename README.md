# Code Retreat - Conway's Game of Life

Today we will be having fun and writing some code! We are going to write a solution to a coding challenge in the language of your choice. The game we will be programming today is [Conway's Game of Life](https://playgameoflife.com/).

![Conway's Game of Life](https://upload.wikimedia.org/wikipedia/commons/e/e5/Gospers_glider_gun.gif)

## Gameplay

Conway's Game of Life is a zero-player game played on a grid. At the start of the game, a pattern is provided as the seed, with dark plots of the grid representing "populated" live cells, and blank plots representing "unpopulated" dead cells. Each subsequent round, the pattern changes based on these [rules](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life#Rules):

1. Any live cell with fewer than two live neighbors dies, as if by underpopulation.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by overpopulation.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

These rules, which compare the behavior of the automaton to real life, can be condensed into the following:

1. Any live cell with two or three live neighbors survives.
2. Any dead cell with three live neighbors becomes a live cell.
3. All other live cells die in the next generation. Similarly, all other dead cells stay dead.

There are various ways to start the game. For our purposes, choose one of the simple patterns provided [here](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life#Examples_of_patterns)

## Coderetreat

A coderetreat is typically a full-day workshop where participants focus on [Extreme Programming](http://www.extremeprogramming.org/) skills of pair programming and test-driven development.

The day is broken down into 45 minute sessions, and during each session, participants work on the same challenge–Conway's Game of Life, but with a new partner and a new _constraint_. That means at the end of each 45 minute session, everything you just wrote will be deleted, and at the beginning of your next session, you will be starting from scratch! After each session we will hold a retro and talk about our takeaways.

### Constraints

Each session will introduce a new constraint. Stand by for more information about that!

## Goals

* Practice with TDD
* Practice with pairing and collaboration
* Learning from eachother
* Comfortability with starting from scratch
* Fast-paced session with new constraints requires quick decision making
* A break from the boring (but important) parts of Welcome Week

## Installation

Choose the language you wish to work on and set up your environment. For the purposes of this workshop, we are going to assume that you are using either Ruby, Python, or JavaScript. Creating the application using a framework (ie: Rails or Django) is not necessary for this activity, as this will just be a quick console application.

To get started, create a directory for our game

```ruby
mkdir code-retreat-gol
cd code-retreat-gol
```

## Tests

Please choose a language with a testing tool that you are familiar with.

#### Ruby

With Ruby, the most common testing tool is [rspec](https://github.com/rspec/rspec-rails), but [minitest](https://github.com/seattlerb/minitest) is another option. You can install these by including the respective gem in a Gemfile.

```ruby
# Gemfile
source "https://rubygems.org"

gem "minitest"
gem "rspec"
```

Then simply bundle your project to install the dependencies

```ruby
bundle install
```

#### Python

[unittest](https://docs.python.org/3/library/unittest.html) is a testing framework included in python's standard library, meaning you can simply include the module in your test file

```
import unittest
```

Another popular option is [pytest](https://docs.pytest.org/en/7.0.x/). You can install pytest using pip.

```python
pip install pytest
```

#### JavaScript

For JavaScript, [jest](https://jestjs.io/) is typically the go-to option. Jest can be installed using yarn

```javascript
yarn add --dev jest
```

Or npm:

```javascript
npm install --save-dev jest
```

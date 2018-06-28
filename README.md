# Startup Penalty Performance Tests

This repository is used to document performance differences between various
programming languages/environments in terms of startup penalty.

## Test Methodology

Each test case represents the shortest possible piece of code to print the string
"Hello World!" and a newline character to stdout.

The performance is measured using the `perf` tool, taking the average of 100
consecutive test runs.

## Structure

The repository is structured as follows:
* A directory for each programming language/environent
    - The code used for the test case
    - A file, `Metadata.md`, describing the parameters used for testing
    - `results.txt`, the raw output of the `perf` command.
* `Metadata.md` in the root directory, specifying the hardware the tests were
  run on.
* This file, `README.md`.

## Results

For the impatient, here's the results of all the tests implemented so far:

|          | Cycles    | Cycles +/- | Time elapsed (ms) | Time elapsed +/- |
|----------|-----------|------------|-------------------|------------------|
| Bash     | 1337075   | 0.10%      | 0.989249          | 0.46%            |
| C        | 249697    | 0.50%      | 0.373877          | 0.54%            |
| C++      | 1760395   | 0.47%      | 1.006922          | 0.42%            |
| Go       | 642472    | 0.57%      | 0.698718          | 1.20%            |
| Node.js  | 201901115 | 0.08%      | 68.112580         | 0.08%            |
| Perl     | 1991706   | 0.46%      | 1.260453          | 0.49%            |
| Python 2 | 26424819  | 0.02%      | 10.0402006        | 0.03%            |
| Python 3 | 57115449  | 0.07%      | 20.373277         | 0.07%            |

# Intro-to-algorithms-project

## Overview
This project calculates the number of sprockets needed to assemble an omnidroid. It uses a dynamic programming approach with memoization to efficiently determine the total cost. The program reads input from a file, processes part dependencies, and recursively computes the total sprocket cost.

## Prerequisites
- Python 3.x installed.
- A text editor or IDE to prepare the input file.

## Libraries Used
- **`defaultdict` from `collections`**: Simplifies managing dependencies as adjacency lists.
- **`sys` module**: Facilitates handling of command-line arguments.

## Input Format
The input file must follow this structure:
1. **First line**: Two integers, `n` and `m`:
   - `n`: Total number of parts.
   - `m`: Number of dependencies between parts.
2. **Next `m` lines**: Each line specifies a dependency as `i j`, meaning part `i` is required to build part `j`.
3. **Final `n` lines**: Each line specifies the sprocket cost for a corresponding part.

## Output Format
The program outputs the total sprockets needed to assemble the omnidroid in this format:
An omnidroid with <n> parts and <m> dependencies takes <total_cost> sprockets to build.

## Running the Program
1. Save the script as `main.py`.
2. Create an input file (e.g., `example-input.txt`) in the same directory as `main.py`.
3. Open a terminal or command prompt, navigate to the directory using `cd`.
4. Run the program with the following command:
   ```sh
   python main.py example-input.txt
  ```
## Example Output
If the input in input-example.txt is:
````sh
8 12
0 1
0 1
0 2
0 2
4 6
5 6
1 7
1 7
2 7
2 7
3 7
6 7
4
2
6
24
14
5
3
6
````

The output will be:
````sh
An omnidroid with 8 parts and 12 dependencies takes 100 sprockets to build.
````


# Map route planner
This is an implementation of the A* search algorithm in C++. A* is an informed search algorithm, which means it uses heuristics to guide the search towards the goal.

## Usage
To use this implementation, you need to provide a path to a file containing a grid of obstacles and free spaces. The file should have one row per line, and each row should contain comma-separated values, where 0 represents a free space and 1 represents an obstacle. The start and goal positions are specified using (x, y) coordinates.

<pre><code>int main() {
  int init[2] = {0, 0};
  int goal[2] = {4, 5};
  auto board = ReadBoardFile("example.txt");
  auto solution = Search(board, init, goal);
  PrintBoard(solution);
}
</code></pre>

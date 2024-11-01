# Dutch Bingo

Dutch Bingo is a C# console application that represents and explores family relationships in a directed labeled graph, with various search features for finding familial connections.

## Features

- **Add Nodes and Relationships**: Adds people and their relationships (e.g., parent, child, spouse) to a graph.
- **Search Relationships**:
  - `Orphans()`: Lists individuals with no recorded parents.
  - `Siblings(name)`: Finds siblings of a specified person.
  - `Descendants(name, depth)`: Lists descendants of a specified person up to a certain depth.
  - `Bingo(name, name2)`: Finds the shortest path between two people.
  - `Cousins(name, degree, removed)`: Finds cousins of a specific relationship level.

## Usage

1. **Load Family Data**:
   Add a .txt file to the correct path with people's names and relationships

2. **Commands**:
   After loading data, the program supports commands like:
   - `ShowPerson name` — displays a person's relationships.
   - `Orphans` — lists all individuals without parents.
   - `Siblings name` — displays siblings.
   - `Descendants name depth` — shows descendants.
   - `Bingo name name2` — finds connections between two people.
   - `Cousins name degree removed` — shows cousins at a given level.
   - If an invalid command is entered, a list of all valid commands will be shown

3. **Exiting**:
   Type `exit` to close the program.

## Example Command Sequence

```plaintext
Enter a command: read relationships.txt
Enter a command: Orphans
Enter a command: Bingo John Mary

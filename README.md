
# Ex.No: 1  Implementation of Breadth First Search 
### NAME : YUVARAJ B                                                                   
### REG NUMBER : 212222040186
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:
```python
graph={
    'A':['B','C'],'B':['D','E'],'C':['F','G'],'D':[],'E':[],'F':[],'G':[]
}
visited=[]
queue=[]
def bfs(visited,graph,node):
    visited.append(node)
    queue.append(node)
    while queue:
        n=queue.pop(0)
        print(n)
        for neighbour in graph:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)
print("Following is the Breath-First Search")
bfs(visited,graph,'A')
```










### Output:
![image](https://github.com/user-attachments/assets/eb9446e9-dc83-4331-a420-8b4332f63739)



### Result:
Thus the breadth first search order was found sucessfully.

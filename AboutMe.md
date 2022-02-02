# Bhargav Reddy Singireddy

I am Bhargav, graduated from SR Engineering college, Warangal, Telangana, India. And statred working as Auto cad Engineer, but gradually developed my interest into computer science and applied for Masters in Computer Science.

[click here to see me](https://github.com/BhargavR12/assignment2-Singireddy/blob/main/Profilepic.jpeg)

---

Adding Table

---

Below table shows the information about the Game and Location about the game and also the price details. 


| Game | Location | Price
| --- | --- | --- |
| Hockey | Carlson Area | 54
| Golf | Andy's GOlf Course | 65
| Rugby | Chester Ground | 77
| Archery | Luckman Place | 34

---

Adding Quotation

---

> “One doesn't expect a falcon to pull a plow, or a butterfly to cook your breakfast.”

― *Katherine Blake, The Interior Life*

> Alex thought about for a minute, chewed his rib eye and simply answered, “yes”

― *L.B. Ó Ceallaigh, Souls' Inverse*

---

Code Fencing

---

> Graph traversal is a subroutine in most graph algorithms. The goal of a graph traversal algorithm is to visit (and / or process) every node of a graph. Graph traversal algorithms, like breadth-first search and depth-first search, are analyzed using the von Neumann model, which assumes uniform memory access cost. This view neglects the fact, that for huge instances part of the graph resides on disk rather than internal memory. Since accessing the disk is magnitudes slower than accessing internal memory, the need for efficient traversal of external memory exists

[Click here for more on Graph Traversal](https://en.wikipedia.org/wiki/External_memory_graph_traversal#:~:text=Graph%20traversal%20is%20a%20subroutine%20in%20most%20graph,Neumann%20model%2C%20which%20assumes%20uniform%20memory%20access%20cost.)

Implemantation for Graph Traversal (Breadth first Search)

~~~

vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}

~~~

[Click here for Source Code](https://cp-algorithms.com/graph/breadth-first-search.html)





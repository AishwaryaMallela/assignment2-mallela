# assignment2-mallela
# Aishwarya
###### Paradise Begumpet

It is famous for ***Biryani's*** and located at the ***center of Hyderabad***.<br>
One of the top most **school** located near the ***metro station***.

---

# Enroute to Paradise from RGIA airport
1. Pick up Shuttle bus Service from RGIA airport.
4. Reach to desination Punjagutta.
    1. Go to nearest metro station.
    2. Buy a ticket to Begumpet station.
6. From Begumpet catch an auto.
8. Reach out to Paradise via CM camp office.
9. Here is the desination for Paradise Biryani Restaurant.
* List of food items
    * Chick Manchurian
    * Prawns fry
    * Chick Biryani
    * Mutton Curry

**[MyImage](AboutMe.md)**

---

## Sport Activity List

Please find below details of sport activities to enroll which consists of name of the sport, location to participate and the amount in dollars for any personal equipment needed.

| Name | Location | Amount |
| :--- | :---: | ---: |
| Basketball | Texas | 140 | 
| Cricket | Kansas | 180 |
| Badminton | Dallas | 120 |
| Football | Atlanta | 100 |
| Hockey | Chicago | 210 |

---

## Pithy Quotes

>You can always edit a bad page. You can’t edit a blank page.<br>
-*Jodi Picoult*

>Meditation is a balancing act between attention and relaxation.<br>-*B. Alan Wallace*

>Mistakes are the portals of discovery<br> -*James Joyce*

---

## Breadth First Search Algorithm

>Breadth-first search (BFS) is an algorithm for searching a tree data structure for a node that satisfies a given property. It starts at the tree root and explores all nodes at the present depth prior to moving on to the nodes at the next depth level. Extra memory, usually a queue, is needed to keep track of the child nodes that were encountered but not yet explored.<br>
<https://en.wikipedia.org/wiki/Breadth-first_search>
```
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
```
<https://cp-algorithms.com/graph/breadth-first-search.html>

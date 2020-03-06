# Lab0

### question 1
* Emily is not eliminated
* Prava is eliminated
* Shashank is not eliminated
* Vicky is eliminated

### question 2
1) Let i and j be elements of the set of teams excluding the team for which we are attempting to determine if it has been eliminated. Let that team be k.

$$ a_{i,j} $$ is the capacity of the edges leading from the source to nodes i_j. Th edges connecting nodes of the form i_j to node i have capacities $$ g_{i,j,i} $$. The edges connecting nodes labeled i to the sink have capacities $$ m_i $$.

$$ a_{i,j} $$ represents the number of games left that team i will play against team j. The edges $$ g_{i,j} $$ also have the capacity of the number of games that teams i and j will play against each other. $$ m_i $$ have values  $$ max(0, w_k + r_k - w_i)

2) $$ a_{prava, vicky} = 2, a_{shashank, vicky} = 0, a_{prava, shashank} = 0, g_{prava, vicky, vicky} = 2, g_{prava, vicky, prava} = 2, g_{shashank, vicky, vicky} = 0, g_{shashank, vicky, shashank} = 0, g_{shashank, prava, shashank} = 0, g_{shashank, prava, prava} = 0, m_{vicky} = 0, m_{prava} = 0, m_{shashank} = 0.

3) Team k is eliminated if the graphs max flow is less than the sum of the capacities of the edges leaving the source.

4) The max flow corresponds to the number of games that can be played while team k still wins. The sum of the outgoing edges is the number of games that will be played. If more games will be played than can occur without team k losing, then team k is eliminated.

### question 3
1) maximize

$$ a_{i,j}, g_{i,j,i}, m_i \geq 0$$ for all i, j


2)

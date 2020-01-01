# Algorithm Study
### 충남대학교 컴퓨터공학과 김진섭  
---------------------------------------------------------------------
# LCS_JAVA
Longest Common Subsequence

input File
-> data1 Length\ndata1\ndata2 Length\ndata2

output File
-> LCS

알고리즘 과제 수행(동적 프로그래밍)
-	과제 목표 : LCS
LCS는 최장 공통 부분 순서를 의미하며 두 문자열 중 공통 부분이 가장 긴 문자열을 뽑아내는 것이다. 이 때 문자열이 연속적일 필요는 없다.

-	해결 방법 : LCS(동적 프로그래밍)
LCS를 재귀적으로 생각하여 보면, X를 x1x2x3x4…로 이루어진 String이고(xa는 char) Y를 y1y2y3…라 한다고 했을 때, xi와 yj에 대하여 생각해보자. 우선 xi와 yj에서의 최장 길이에 대한 데이터 정보가 담긴 값으로 cij가 있다고 하자. 우리가 유의해 살펴보며 찾아야하는 값은 cij이다.
만약, I 또는 j가 0이있는 경우에는 두 문자열 중 하나가 문자가 아무것도 없는 경우이므로 0을 넣어준다.
만약 xi와 yj가 같은 경우라면 cij는 c(i-1)(j-1)에서 1을 더해준 값이 된다.
만약 두 값이 서로 다른 경우라면, c(i-1)j나 ci(j-1)중에서 큰 값이 들어가게 될 것이다.
위 방법대로 재귀적으로 사용을 하게 되면, 심한 중복 호출이 발생한다. 따라서, 이를 해결하기 위해서는 구해준 cij에 대한 정보를 0에서부터 차례대로 삽입하며 테이블을 형성해야한다.
---------------------------------------------------------------------
# Dijkstra_Bellman-Ford_Java 

[알고리즘] 다익스트라와 벨만포드 알고리즘 구현

#### 다익스트라
최단 경로를 찾아내는 알고리즘
음의 간선이 존재하는 경우 다익스트라가 원활히 수행이 안됨


#### 벨만포드
최단 경로를 찾아내는 알고리즘
음의 사이클이 존재하는 경우 벨만포드가 원활히 수행이 안됨

---------------------------------------------------------------------
# DFS_BFS_JAVA

## DFS와 BFS 구현
[알고리즘] 깊이우선탐색과 너비우선탐색 알고리즘 구현

#### DFS
깊이우선 탐색 알고리즘  

#### BFS
너비우선 탐색 알고리즘

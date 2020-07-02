# 새로운 디자인에 대한 제안

## "이주열"의 자기소개

**이주열**은 어떤 사람인가요?

### 표 완성해보기



```markdown
이번학기 수강과목

* 1.스포츠마사지
* 2.소프트웨어 공학 개론
* 3.오픈소스 소프트웨어
* 4.컴퓨터 데이터구조
* 5.프로그래밍응용1
```
### 존경하는 인물의 사진과 그 인물의 명언

![빌 게이츠](/bill.jpg "빌 게이츠")

> ″성공은 형편없는 선생님이다. 똑똑한 사람들을 실패할 수 없다는 착각에 빠트린다.”

### 내가 최근에 사용해본 코드   
```python
class Node:
  def __init__(self, data):
    self.data = data
    self.neighbors = []
    self.visited = False
    
  def add_neighbor(self, neighbor):
    self.neighbors.append(neighbor)

  def set_visited(self, visited):
    self.visited = visited

  def get_data(self):
    return self.data

  def get_neighbors(self):
    return self.neighbors

  def get_visited(self):
    return self.visited


class Graph:
  def __init__(self):
    self.nodes = []

  def add_node(self, node):
    self.nodes.append(node)
  
  def topological_sort(self):
    if len(self.nodes) > 0:
      for node in self.nodes:
        node.set_visited(False)

      self.stack = []
      for i in range(len(self.nodes)):
        self.sequence(self.nodes[i])
      for i in range(len(self.stack)):
        print(self.stack.pop())
    print("")

  def sequence(self, node):
    if node.get_visited() == True:
      pass
    else:
      node.set_visited(True)
      neighbors = node.get_neighbors()
      if len(neighbors) > 0:
        for i in range(len(neighbors)):
          self.sequence(neighbors[i])
      self.stack.append(node.get_data())
     
graph = Graph()

node_A = Node('A')
graph.add_node(node_A)
node_B = Node('B')
graph.add_node(node_B)
node_C = Node('C')
graph.add_node(node_C)
node_D = Node('D')
graph.add_node(node_D)
node_E = Node('E')
graph.add_node(node_E)
node_F = Node('F')
graph.add_node(node_F)
node_G = Node('G')
graph.add_node(node_G)
node_H = Node('H')
graph.add_node(node_H)
node_I = Node('I')
graph.add_node(node_I)
node_J = Node('J')
graph.add_node(node_J)

node_A.add_neighbor(node_B)
node_A.add_neighbor(node_F)

node_B.add_neighbor(node_H)

node_D.add_neighbor(node_C)
node_D.add_neighbor(node_E)
node_D.add_neighbor(node_I)

node_E.add_neighbor(node_I)

node_G.add_neighbor(node_A)
node_G.add_neighbor(node_B)
node_G.add_neighbor(node_C)

node_I.add_neighbor(node_C)

node_J.add_neighbor(node_E)

graph.topological_sort()

```

### 나의 깃허브 주소
[여기](https://github.com/tyr1028/Leejooyeol.github.io "이주열의 깃허브")

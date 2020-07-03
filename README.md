# Team-2 Members Self-Introduntion

-----
## Minsoo Kim's self-introduction

### **Who is Minsoo Kim?**

|Date of birth|E-mail|
|:----|:-----|
|06th August 1998|alstn9008@gmail.com|

### Bucket List

* **Personal** garage
* *Muscle car*
* **Be a softwareEngineer**

### Idol and his quote

![George patton](https://upload.wikimedia.org/wikipedia/commons/7/75/General_George_S._Patton_wearing_his_4-star_service_cap.jpg)
> Accept challenges, so that you may feel the exhilaration of victory -George patton-

### Lastest Code
```python
from random import randint

play = ["Rock", "Paper", "Scissors"]
print('Computer: {}'.format(computer))

play = input("Rock, Paper, Scissors? ")
print('Player: {}'.format(computer))
```
### Github address
[*MinsooKim's Github*](https://github.com/alstn9008/)

-----
# TEAM-2의 자기소개


## "이주열"의 자기소개

**이주열**은 어떤 사람인가요?

### 표 완성해보기
| 카테고리      | 정보 |
|---------------|--------|
| 좋아하는 색깔 | 파란색 |
| 좋아하는 음식 | 달달한 음식|
|취미 | 게임과 제빵|

```markdown
이번학기 수강과목

* 1.스포츠마사지
* 2.소프트웨어 공학 개론
* 3.오픈소스 소프트웨어
* 4.컴퓨터 데이터구조
* 5.프로그래밍응용1
```
### 존경하는 인물의 사진과 그 인물의 명언

![빌 게이츠](/https://upload.wikimedia.org/wikipedia/commons/2/2d/Bill_Gates_2014.jpg)

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


------
## "김종한"의 자기소개

**김종한**은 어떤 사람인가요?

### 표 완성해보기

|좋아하는 음식|취미|존경하는 인물|가장 아끼는 물건|
|:-----:|:-----:|:-----:|:-----:|
|아이스크림|넷플릭스보기|리처드 파인만|노트북|

### 버킷 리스트
* 번지점프   
* 세계여행    
* 게임 제작해보기   
* 일본에서 2년 이상 생활하기  


### 존경하는 인물의 사진과 그 인물의 명언
![사진]( http://image.dongascience.com/Photo/2016/12/14810989645256.jpg "인물사진")

> 신은 불가사의를 설명하기 위해 만들어진다. 사람들은 이해되지 않는 것들을 설명하기 위해 신을 만들었다. 하지만 마침내 세상이 움직이는 원리를 알게 된다면,신으로부터 벗어나는 방법을 터득하게 된 것이며, 더 이상 신은 필요 없다. -리처드 파인만

### 내가 최근에 사용해본 코드   
```markdown
# Welcome to OSS-team-2 Pages
리스트는 이렇게 만듭니다
* 리스트1
* 리스트2
* 리스트3

```


### 나의 페이스북 주소   
[김종한의 페이스북 바로가기]( https://www.facebook.com/profile.php?id=100010597456027 "김종한의 페이스북")

-----
## "이지은"의 자기소개

**이지은**은 어떤 사람인가요?

### 표 완성해보기

좋아하는 것에 대해서

|음식|영화|드라마|음악|스포츠|게임|동물|취미|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|망고|해리포터|미스터션샤인|Yellow-Coldplay|축구|카트라이더|강아지|영화보기|

### 버킷리스트
+ 스페인에 가서 축구경기 직관하기
+ 시베리아횡단열차타기
+ 반려동물데리고 바닷가가기

### 인생 좌우명
> 남의 불행을 나의 위안으로 삼지말자

### 좋아하는 영화배우
![Cillian Murpy](https://user-images.githubusercontent.com/65939621/86267714-1bc3e180-bc02-11ea-9e87-e55d0ee1430c.jpg)

### 내가 최근에 사용해 본 코드
```python
import sys

class Node:

  index = 0

  def __init__(self, data): 
    self.index = Node.index
    Node.index += 1
    self.data = data
    self.neighbors = []

    self.key = sys.maxsize
    self.memo = None
    self.is_done = False

  def get_index(self):
    return self.index

  def get_data(self):
    return self.data

  def get_neighbors(self):
    return self.neighbors
```

### 나의 github 홈페이지 주소
[이지은의 github홈페이지](https://zinneylee.github.io/)

-----
## "김민지"의 자기소개

**김민지**은 어떤 사람인가요?

### 표 완성해보기

좋아하는 것에 대해서

|음식|영화|드라마|음악|스포츠|게임|동물|취미|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|스파게티|호러물|싸이코지만괜찮아|발라드|요가|오버워치|고양이|게임하기|

### 버킷리스트
+ 스쿠버다이빙
+ 스카이다이빙
+ 번지점프

### 인생 좌우명
> 약속을 지키자

### 좋아하는 영화배우
![Cillian Murpy](https://img1.daumcdn.net/thumb/R800x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F12472D2E4C725F8F08)
### 내가 최근에 사용해 본 코드
```python

```

### 나의 github 홈페이지 주소
[김민지의 github홈페이지](https://github.com/mminji-kim)

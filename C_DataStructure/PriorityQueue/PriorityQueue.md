# 우선순위 큐 (Priority Queue)

## Priority Queue란?
  - 우선순위가 높은 데이터가 먼저나오고, 우선순위가 낮은 데이터가 나중에 나오도록 하는 자료구조이다.

## Priorit Queue의 조건
  - 우선순위를 사용자가 목적에 맞게 정해야 한다.
  - 데이터를 근거로, 우선순위를 판단할 수 있어야 한다.
  - 우선순위가 같은 데이터가 존재할 수도 있다.

## Priority Queue의 구현

### 1. 배열을 이용한 구현
  - 데이터의 저장과 삭제 과정에서 번거로운 연산들이 생겨난다.
  - 데이터 삽입을 위해서, 배열에 저장된 모든 데이터들과 값을 비교 해야하는 상황이 발생할 수도 있다 : 과다 연산

### 2. 연결 리스트를 이용한 구현
  - 데이터의 삽입을 위해서, 연결 리스트에 저장된 모든 데이터들과 값을 비교 해야하는 상황이 발생할 수도 있다 : 마찬가지로 과다 연산

### 3. 힙(heap)을 이용한 구현
  - **priority queue를 구현하기 위해서 가장 일반적으로 사용하는 자료구조**이다.
  - 데이터가 두배 증가할때마다, 연산횟수가 1 증가하므로, 과다한 연산으로 인한 부하를 방지할 수 있다.

 |시간 복잡도|삭제|삽입|
 |:---:|:---:|:---:|
 |배열 기반|O(1)|O(N)|
 |연결리스트 기반|O(1)|O(N)|
 |힙 기반|O(log2N)|O(log2N)|

## Heap을 이용한 Priority Queue의 구현
  - **root 노드 쪽에 존재하는 데이터일수록 우선순위가 높아지도록 Heap자료구조를 이용하는 것**이다!
    - Heap 자료구조 자체는 max Heap과 min Heap이 존재한다 : 노드의 데이터값이 max Heap은 root로 갈수록 커지고, min Heap은 root로 갈수록 작아진다.
    - max Heap 또는, min Heap을 이용하여 우선순위에 대한 기준을 정하여 Heap 자료구조를 priority queue라는 목적에 맞게 이용하는 것이다.



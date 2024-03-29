## Segment Tree

### 언제 쓰는가?
  - 연속된 데이터들에 대한 빠른 시간 내의 탐색, 수정, 추가, 삭제 연산을 가능하게 해준다.
  - 특히, **"특정 구간 내의 최대값, 최소값, 데이터들의 합"을 구하는 연산을 빠르게 수행**할 수 있다.
    - 특정 구간에서의 합, 최대값, 최소값에 대한 정보를 미리 트리로 구성해두고 필요에 따라 꺼내쓴다.
    - 데이터의 갯수 * 4 정도의 공간을 미리 마련해두어야 한다.

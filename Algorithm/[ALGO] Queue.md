# Queue
  > **먼저 들어온 게 먼저 나오는 FIFO (First-In First-Out) 형태의 자료 구조**
  
  Queue는 스택과 반대되는 개념으로, 먼저 들어온 값이 먼저 나오는 FIFO 형태의 자료 구조이다.  
  대기열을 생각하면 쉽다.  
  **(대기열은 먼저 들어온 사람이 먼저 나가지 않는가?)**  
  ![](https://img.newspim.com/news/2023/02/01/230201164600129_w.jpg)

  ## Queue의 종류
  - **선형 큐** - 흔히 볼 수 있는 큐로, 단어 그대로 선형으로 된 큐이다.
  - **원형 큐** - 선형 큐의 문제점을 보완하기 위한 자료구조로, 포인터 증가 방식이 변화되어 배열의 첫 인덱스부터 데이터 삽입이 가능해진 큐이다.
  - **우선순위 큐** - 우선순위가 높은 데이터가 먼저 나가는 형식의 큐이다.

  ## Queue의 연산
  **size() -** 큐에 들어 있는 데이터 원소 개수를 반환한다.  
  **isEmpty() -** 큐가 비어 있는지를 판단한다.  
  비어있으면 True를 비어있지 않으면 False를 반환한다.  
  **push(x) -** 큐의 오른쪽(끝)에 데이터 x를 추가한다.  
  **pushleft(x) -** 큐의 왼쪽(시작)에 데이터 x를 추가한다.  
  **pop() -** 큐의 맨 오른쪽(끝)의 데이터 원소를 반환하고, 제거한다.  
  **popleft() -** 큐의 맨 왼쪽(시작)의 데이터 원소를 반환하고, 제거한다.  
  **peek() -** 큐의 맨 끝의 데이터 원소를 반환한다.  

  ## Queue의 장/단점
  - ### 장점
    - 데이터의 순서가 중요한 작업에서 유용하게 쓸 수 있다.
    - 덱(Deque)을 사용하면 양 끝에서의 삽입과 삭제가 가능하다.

  - ### 단점
    - 큐의 크기가 고정되 있을 때, 데이터가 다 차면 더 이상 삽입이 불가하다.
    - 덱(Deque)은 메모리 사용량이 크다.

  ## Queue의 사용처
  - **캐시 구현**
  - **프린터 인쇄 대기열**
  - **너비 우선 탐색**
  - **프로세스 관리**
  - **CPU 스케줄링**

  ## Queue 면접 에상 질문
  - **큐는 어떤 상황에서 사용될까요?**
  - **우선순위 큐는 어떻게 구현하는가?**
  - **큐의 종류와 특징을 설명하시오.**
  - **너비 우선 탐색(BFS)를 구현할 수 있는가?**
  - **2개의 Stack으로 Queue를 구현할 수 있는가?**
# Stack
  > **한 쪽 끝에서만 자료를 넣고 뺄 수 있는 LIFO(Last In First Out) 형식의 자료 구조**

  Stack은 위 설명처럼 **한쪽에서만 자료를 넣고 뺄 수 있는 LIFO 형식**의 자료 구조이다.  
  팬케이크 탑을 떠올려보면 이해가 쉽다.
  ![](https://i.namu.wiki/i/sonbaPfQD9CKqe0nOHHEd2CW-w-it6pyjWq-iQlDsGQHj47gQRBRPBn8Bl_42R9bYPBPKdWBtGXkAXNkqNfVYg.webp)  
  (팬케이크는 보통 위 것부터 먹는다)

  ## Stack의 연산
  **size() -** 현재 스택에 들어 있는 데이터 원소 개수를 반환한다.  
  **isEmpty() -** 현재 스택이 비어 있는지를 판단한다.  
  비어있으면 True를 비어있지 않으면 False를 반환한다.  
  **push(x) -** 스택에 데이터 x를 추가한다.  
  **pop() -** 스택의 맨 위의 데이터 원소를 반환하고, 제거한다.  
  **peek() -** 스택의 맨위의 데이터 원소를 반환한다.  

  ## Stack의 사용처
  - **재귀 알고리즘**
  - **웹 브라우저 방문기록 (뒤로가기)**
  - **실행 취소 (undo)**
  - **역순 문자열 만들기**
  - **수식의 괄호 검사 (연산자 우선순위 표현을 위한 괄호 검사)**
  - **후위 표기법 계산**

  ## Stack 면접 에상 질문
  - **스택은 어떤 상황(알고리즘)에서 어떻게 사용될까요?**
  - **사용 언어에서 스택 구현할 수 있는가? 어떤 함수 사용?**
  - **메모리 구조에서 스택의 역할은?**
  - **깊이 우선 탐색(DFS)에서 어떻게 사용되는가?**
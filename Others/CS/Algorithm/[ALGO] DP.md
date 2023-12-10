# DP
  > **큰 문제를 작게 나눠 효율적으로 해결하는 기법**
  
  복잡한 문제를 간단한 여러 문제로 나누어 푸는 기법이다.
  
  부분 문제 반복과 최적 부분 구조를 가지는 알고리즘을 풀 때 사용하며, 분할 정복 알고리즘으로 분류되어있다.  

  ## 종류
  - ### Bottom-Up
    반복문을 사용하여 작은 문제부터 답 도출  
    Tabulation

  - ### Top-Down
    큰 문제를 해결하기 위해 재귀 함수 호출  
    Memoization

  ## DP 테이블 초기화
  DP를 할 때는 DP 테이블을 무조건 초기화해야 한다.

  그 후 필요한 값들을 삽입하여 사용한다.
# 2020-2학기 자료구조 수업 (실습 코드 정리)

1. 자료구조와 알고리즘 개략적인 이해
 * 자료구조 : 컴퓨터에서 자료를 정리하고 조직화하는 다양한 구조
   + 단순 자료구조 : 정수, 실수, 문자, 문자열, 포인터
   + 복합 자료구조 
       - 선형 구조 : 스택, 큐, 덱, 리스트
       - 비선형 구조 : 트리, 우선순위 큐, 그래프 ,맵

 * 알고리즘 : 컴퓨터로 문제를 풀기 위한 단계적인 절차
   + 조건 
      - 입  력 : 0개 이상의 입력이 존재하여야 한다. 
      - 출  력 : 1개 이상의 출력이 존재하여야 한다. 
      - 명백성 : 각 명령어의 의미는 모호하지 않고 명확해야 함.
      - 유한성 : 한정된 수의 단계 후에는 반드시 종료되어야 함.   
      - 유효성 : 각 명령어들은 실행 가능한 연산이어야 한다.

   + 기술 방법 
       - 자연어  : 읽기 쉽다 ↔ 의미 전달이 모호
       - 흐름도(flow chart) : 직관적, 이해하기 쉬움 ↔ 복잡한 경우 표시가 복잡
       - 유사 코드(pseudo-code) : 알고리즘의 핵심적인 내용에만 집중 ↔ 구현 문제들을 감출 수 있음 (자연어보다 구조적, 플밍 언어보다 덜 구체적) 
       - 특정 프로그래밍 언어 : 알고리즘의 가장 정확한 기술 가능 ↔ 구체적인 사항들이 알고리즘의 핵심적인 내용들의 이해를 방해 가능

 * 자료형과 추상 자료형
   + 추상 자료형(ADT: Abstract Data Type) : 객체 + 연산
       - 데이터 타입을 추상적(수학적)으로 정의한 것
       - 데이터나 연산이 무엇(what)인가를 정의함
       - 데이터나 연산을 어떻게(how) 구현할 것인지는 정의하지 않음

  + 추상 자료형과 C++
       - 추상 자료형의 개념은 객체지향의 개념과 정확히 일치한다. 
       - 객체지향언어인 C++에서는 클래스를 사용하여 추상 자료형을 구현한다. 
       - 추상 자료형에서의 “객체”는 클래스의 속성(멤버 변수)으로 구현되고 “연산”은 클래스의 메소드(멤버 함수)로 구현된다. 
       - C++에서는 private나 protected 키워드를 이용하여 속성과 연산에 대한 접근을 제한할 수 있다.
       - 클래스는 계층구조(상속)로 구성될 수 있다. 

 * 알고리즘의 성능분석
  + 실행시간 측정
  + 복잡도를 분석
       - 시간 복잡도 분석 T(n) : 수행 시간 분석 → 빅오 표기법
         A. 빅오 표기법 O(g(n)) : 두 개의 함수 f(n) & g(n), 모든 n≥n0에 대하여 |f(n)| ≤ c|g(n)|을 만족하는 2개의 상수 c와 n0가 존재하면 f(n)=O(g(n))이다.   
          ㄴ 순서 : 1	logn	n	nlogn	n2	n3	2n	n!   
         B. 빅오메가 표기법 Ω(g(n)) : 하한을 표시   
         C. 빅세타 θ(g(n)) : 하한인 동시에 상한을 표시   
         D. 최선, 평균, 최악의 경우   
           a. 최선의 경우(best case): 수행 시간이 가장 빠른 경우 - 의미 없는 경우 多   
           b. 평균의 경우(average case): 수행시간이 평균적인 경우 - 계산이 어려움   
           c. 최악의 경우(worst case): 수행 시간이 가장 늦은 경우 - 가장 널리 사용   

       - 공간 복잡도 분석 : 수행시 필요로 하는 메모리 공간 분석

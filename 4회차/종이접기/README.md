# 종이접기
## 문제
크기가 N X M 인 종이를 계속 접어 크기가 1 X 1 이 될 때까지 접은 후 이를 펼치면 종이엔 줄무늬가 생긴다. 어떤 줄무늬는 위로 볼록하고, 어떤 것은 아래로 볼록한 모양을 띄게 된다. 위로 볼록한 무늬를 굵은 실선으로, 아래로 볼록한 무늬를 굵은 점선으로 나타내자. 아래 그림은 2 X 3 크기의 종이를 어떤 순서로 접었나에 따른 서로 다른 줄 무늬를 보여주고 있다.

![그림 1](./img/paper1.png)

격자의 정보를 나타내는 자연수 N과 M, 그리고 줄무늬를 나타내는 정보가 주어질 때, 그런 무늬가 실제로 종이를 접은 후 펼쳐서 얻어진 그림인지, 아니면 인위적으로 그린 그림인지를 판단하는 프로그램을 작성하시오.

### 입력 형식
첫째 줄에 테스트 케이스의 수 T (1 ≤ T ≤ 10)가 주어진다. 각 테스트 케이스의 첫째줄엔 종이의 세로 크기를 나타내는 정수 N(2 ≤ N ≤ 50)과 가로 크기를 나타내는 정수 M(2 ≤ M ≤ 50)이 주어진다. 이어지는 N줄 각각엔 M-1 개의 정수(0 또는 1)가 주어지는데 이는 격자의 세로방향 무늬에 대한 정보이다. 즉, i 번째 줄에 있는 M-1개 정수는 격자의 i 번째 행에 있는 M-1개의 세로 방향에 관한 무늬 정보이다. 1은 위로 볼록한 무늬를, 0은 아래로 볼록한 무늬를 의미한다. 이어지는 N-1 줄 각각엔 M 개의 정수(0 또는 1)가 주어지는데 이는 가로방향 무늬에 대한 정보이다. 즉, i 번째 줄에 있는 M 개 정수는 격자의 i 번째 행에 있는 M 개의 가로 방향에 관한 무늬 정보이다. (아래 그림 참조)
![그림 2](./img/paper2.png)

### 출력 형식
한 줄로 결과를 출력한다. 주어진 무늬 정보가 실제로 종이를 접은 후 펼쳐서 얻어지는 것이면 1, 그렇지 않으면 0을 출력한다.

### 입력 예제 1
> 2  
> 2 3  
> 1 1  
> 1 1  
> 0 1 0  
> 4 6  
> 1 0 1 1 0  
> 0 1 0 0 1  
> 1 0 1 1 0  
> 0 1 0 0 1  
> 1 1 1 1 1 1  
> 1 1 1 1 1 1  
> 1 1 1 1 1 1  

### 출력 예제 1
> 1 1

### 입력 예제 2
> 2  
> 2 3  
> 1 0  
> 1 0  
> 1 0 1  
> 4 6  
> 1 0 1 1 0  
> 0 1 0 0 1  
> 1 0 1 1 0  
> 0 0 0 0 1  
> 1 1 1 1 1 1  
> 1 1 1 1 1 1  
> 1 1 1 1 1 1  

### 출력 예제 2
> 1 0

### 입력 예제 3
> 1  
> 2 4  
> 0 1 1  
> 1 1 0  
> 1 1 1 0  

### 출력 예제 3
> 0

### 채점 방식
입력 케이스들은 다음과 같은 종류로 구별되며, 한 종류의 케이스를 다 맞추어야 그 종류에 배정된 점수를 받을 수 있다.

* 종류 1 (20점): N = M = 2 이다.
* 종류 2 (55점): 세로무늬 값은 모두 1이다.(즉, 세로선은 모두 위로 볼록하다.)
* 종류 3 (125점): 별다른 제약조건 없음.

### 제한 사항
|     언어     |  시간 제한   | 메모리 제한  |
|:------------:|:------------:|:------------:|
|       C      |     1.5초    |    256MB     |
|     C(11)    |     1.5초    |    256MB     |
|      C++     |     1.5초    |    256MB     |
|    C++(11)   |     1.5초    |    256MB     |
|    C++(14)   |     1.5초    |    256MB     |
|    C++(17)   |     1.5초    |    256MB     |
|      C#      |     1.5초    |    256MB     |
|     JAVA     |     1.5초    |    256MB     |
|    Python2   |     1.5초    |    256MB     |
|    Python3   |     1.5초    |    256MB     |

## 풀이

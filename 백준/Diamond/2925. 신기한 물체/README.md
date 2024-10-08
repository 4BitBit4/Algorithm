# [Diamond II] 신기한 물체 - 2925 

[문제 링크](https://www.acmicpc.net/problem/2925) 

### 성능 요약

메모리: 2028 KB, 시간: 64 ms

### 분류

값 / 좌표 압축, 자료 구조, 느리게 갱신되는 세그먼트 트리, 수학, 정수론, 오프라인 쿼리, 세그먼트 트리

### 제출 일자

2024년 10월 2일 16:32:44

### 문제 설명

<p>어느 날, 상근이는 길을 걷던 중에 신기한 물체를 발견했다. 외계의 것으로 추정되는 이 물체의 왼편에는 빈 박스가 N개 있었다. 기계의 사용방법을 알아내기 위해서 하루종일 기계를 더듬거렸고, 마침내 상근이는 이 기계를 어떻게 사용하는지를 알게되었다.</p>

<p>기계는 정수 4개 L, R, A, B를 입력으로 받는다. 크고 빨갛게 빛나는 실행버튼을 누르면 기계는 다음과 같은 움직인다.</p>

<p>먼저, L번 박스에 들어 있는 돌의 개수를 A mod B개로 만든다. 그 다음 L+1번 박스에 들어 있는 돌을 (2*A) mod B개로 만든다. 마찬가지로, L+2번 박스에 들어 있는 돌을 (3*A ) mod B개로 만든다. 즉, L번과 R번 사이의 X번 박스에 들어 있는 돌의 개수를 ((X-L+1)*A) mod B개로 만드는 것이다. R번 박스까지 돌을 채우고나면, 기계는 다음 명령을 기다린다.</p>

<p>기계에 여러 가지 명령을 내리던 중에, 상근이는 어떤 박스의 구간에 들어있는 돌의 개수가 궁금해졌다.</p>

<p>상근이가 기계에 입력한 명령이 주어졌을 때, 이 기계를 시뮬레이팅 하면서, 상근이의 궁금증도 해결해주는 프로그램을 작성하시오.</p>

### 입력 

 <p>첫째 줄에 박스의 수 N과 쿼리의 수 Q가 주어진다. (1 ≤ N ≤ 1,000,000,000, 1 ≤ Q ≤ 50,000)</p>

<p>다음 Q개 줄에는 시뮬레이션에 관한 정보가 주어진다.</p>

<p>만약, 정보가 1로 시작한다면, 형식은 "1 L R A B" (1 ≤ L ≤ R ≤ N, 1 ≤ A, B ≤ 1,000,000)가 된다. 이 뜻은 상근이가 기계에 L, R, A, B를 입력했다는 뜻이다.</p>

<p>정보가 2로 시작한다면, 형식은 "2 L R"이 된다. (1 ≤ L ≤ R ≤ N) 이 뜻은 상근이가 L과 R번 박스 사이에 들어있는 돌의 개수를 궁금했다는 뜻이고, 개수를 구한뒤, 출력해야 한다. L과 R도 범위에 포함된다.</p>

### 출력 

 <p>2로 시작하는 명령이 들어올 때 마다, 그 구간에 들어있는 돌의 개수를 출력한다.</p>


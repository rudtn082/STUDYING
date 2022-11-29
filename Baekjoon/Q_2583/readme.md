# 영역 구하기(2583번)  

### 문제  
눈금의 간격이 1인 M×N(M,N≤100)크기의 모눈종이가 있다. 이 모눈종이 위에 눈금에 맞추어 K개의 직사각형을 그릴 때, 이들 K개의 직사각형의 내부를 제외한 나머지 부분이 몇 개의 분리된 영역으로 나누어진다.  

예를 들어 M=5, N=7 인 모눈종이 위에 <그림 1>과 같이 직사각형 3개를 그렸다면, 그 나머지 영역은 <그림 2>와 같이 3개의 분리된 영역으로 나누어지게 된다.  

![문제이미지](/img/2583image.png "문제이미지")  

M, N과 K 그리고 K개의 직사각형의 좌표가 주어질 때, K개의 직사각형 내부를 제외한 나머지 부분이 몇 개의 분리된 영역으로 나누어지는지, 그리고 분리된 각 영역의 넓이가 얼마인지를 구하여 이를 출력하는 프로그램을 작성하시오.  

### 입력  
첫째 줄에 M과 N, 그리고 K가 빈칸을 사이에 두고 차례로 주어진다. M, N, K는 모두 100 이하의 자연수이다. 둘째 줄부터 K개의 줄에는 한 줄에 하나씩 직사각형의 왼쪽 아래 꼭짓점의 x, y좌표값과 오른쪽 위 꼭짓점의 x, y좌표값이 빈칸을 사이에 두고 차례로 주어진다. 모눈종이의 왼쪽 아래 꼭짓점의 좌표는 (0,0)이고, 오른쪽 위 꼭짓점의 좌표는(N,M)이다. 입력되는 K개의 직사각형들이 모눈종이 전체를 채우는 경우는 없다.  

### 출력  
첫째 줄에 분리되어 나누어지는 영역의 개수를 출력한다. 둘째 줄에는 각 영역의 넓이를 오름차순으로 정렬하여 빈칸을 사이에 두고 출력한다.  

### 느낀점  
내가 풀었던 풀이 방법은 먼저 이중 배열을 만들어서 0으로 초기화한다.  
그리고 도형이 있는 부분은 좌표를 분석하여 1로 변경해준다.  
좌표가 완성된 이후 0이면서 인접 좌표 검사를 하지 않은 좌표에 대해서 인접 0에 대하여 찾으면서 넓이를 구한다.  
넓이를 모두 구한 후 정렬하고 출력한다.  

정답이 제대로 출력되는데, 자꾸 틀렸다고 나왔다. 왜 그런지 몰라서 많이 헤맸는데 이유는 오름차순 정렬을 잘못했었다....  
정렬이 틀릴 줄은 몰라서 안 보고 있었는데 앞으로 코드를 자세히 봐야겠다.  

그리고 나는 코드 길이가 4211B인데 맞은 사람의 대부분이 2~3000B 정도로 나오는 것 같다.  
좀 더 효율적인 코딩이 필요하다고 느꼈다!  
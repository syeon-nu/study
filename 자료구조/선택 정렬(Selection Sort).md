# 선택 정렬
1. 아직 정렬되지 않은 숫자들 중에서 가장 작은 숫자를 찾는다.
2. 그 숫자를 정렬된 부분의 맨 끝에 놓는다.
3. 이 과정을 모든 숫자가 정렬될 때까지 반복

``` c
// 선택 정렬 구현하기
void selectionSort(int list[], int n) {
    int i, j, min, temp;
    
    // 외부 반복문: 정렬할 위치를 이동합니다 (0부터 n-2까지)
    for (i = 0; i < n-1; i++) {
        // min에 현재 위치(i)를 저장한다
        min = i;
        
        // 내부 반복문: i+1부터 끝까지 검사하며 최솟값 찾기
        for (j = i+1; j < n; j++) {
            // 현재 min보다 더 작은 값을 발견하면
            if (list[j] < list[min]) {
                // min 위치를 업데이트
                min = j;
            }
        }
        
        // i번째 값과 찾은 최솟값을 교환한다
        if (min != i) { // 최솟값이 i와 다르면 교환 필요
            temp = list[i];
            list[i] = list[min];
            list[min] = temp;
        }
    }
}
```

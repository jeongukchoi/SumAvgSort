# 내일배움캠프 언리얼 - C++ 과제 1
** 링크는 12.26에 제출하였으나 12.27에 마지막으로 수정되었습니다 **

## 필수 기능
- 사용자로부터 5개의 숫자를 입력 받아 배열에 저장하고 이들의 합계와 평균을 계산해서 출력해주세요!
  > ArrayHandler 클래스 : 사용자 입력이 유효한지 체크해 배열에 저장 / 현재 배열의 원소 출력
   
  > Calculator 클래스 : 합계 / 평균 계산 후 반환

- 5개의 숫자를 입력 받는 공간은 배열을 활용할게요!
- 합과 평균을 구하는 동작은 main함수에 한번에 작성하지 말고 각각 함수를 구현해주시는 것으로 해요!
    - 왜 이렇게 하는 것이 좋은지를 한 번 더 생각해보면서 작성해봐요!

## 도전 기능
도전 기능인만큼 난이도가 쉽지는 않아요! 사용자가 입력한 숫자 배열을 정렬하는 프로그램을 구현해볼까요?
- 정렬은 오름차순 정렬과 내림차순 정렬이 가능해야 합니다.
- 숫자 1을 입력 받으면 오름차순 정렬, 숫자 2를 입력 받으면 내림차순 정렬을 하도록 구현해주세요.
    - 입력을 구현하는 방법은 원격강의에서 배울겁니다!
- `algorithm` 헤더의 `sort` 함수를 사용하지 않고 직접 구현해보세요.
- 오름차순 정렬과 내림차순 정렬 동작을 각각 함수로 구현해봐요!
 > Sorter 클래스 : 현재 배열을 사용자 입력에 따라 오름차순 또는 내림차순 정렬 / 합병 정렬 알고리즘 구현

  > void mergeSort() : 합병 정렬 (참고한 자료: https://www.youtube.com/watch?v=3j0SWDX4AtU)
  > 1. 배열을 재귀적으로 왼쪽과 오른쪽 절반으로 나눈다.
  > 2. 쪼개어진 절반의 크기가 1이 되었을 때 base case로 바로 전 단계로 return.
  > 3. 재귀가 끝난 시점에 merge()를 이용해 정렬 순서에 맞게 두 배열을 하나로 합친다.
  
  > void merge() : mergeSort() 에서 호출하는 헬퍼 메서드
  > 두 배열의 원소인 숫자의 크기를 비교하고 정렬 순서에 따라 알맞게 배치해 원본 배열에 저장한다.
  > 오름차순인 경우 두 배열의 현재 원소(정수)를 비교해 작은 숫자를 원본 배열의 현재 위치에 배치한다.
  > 내림차순인 경우 두 배열의 현재 원소(정수)를 비교해 큰 숫자를 원본 배열의 현재 위치에 배치한다.

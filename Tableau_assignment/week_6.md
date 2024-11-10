# Sixth Study Week


## Study Schedule
<br>

| 회차 | 강의 범위   | 강의 이수 여부 | 링크                                                                                                     |
|------|-------------|----------------|--------------------------------------------------------------------------------------------------------|
| 1    | 1~7강       | ✅              | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=84)    |
| 2    | 8~17강      | ✅              | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=75)    |
| 3    | 18~27강     | ✅              | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=65)    |
| 4    | 28~37강     | ✅              | [링크](https://www.youtube.com/watch?v=e6J0Ljd6h44&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=55)    |
| 5    | 38~47강     | ✅              | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=45)    |
| 6    | 48~57강     | ✅              | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=35)    |
| 7    | 58~67강     | 🍽️             | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=25)    |
| 8    | 68~77강     | 🍽️             | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=15)    |
| 9    | 78~85강     | 🍽️             | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=5)     |
---

<br/>
<!-- 여기까진 그대로 둬 주세요-->

> **🧞‍♀️ 오늘은 강의보다 실습과 대시보드 직접 만들기가 더 중요하니, 기록보다는 사고하며 강의를 들어주세요.**

## 48. 워크시트 서식(2)
<!-- 워크시트에 관해 본 강의에서 알게 된 점을 적어주세요 -->


**테두리**

![alt text](../image/6주차/48강-테두리.png)



**라인**

![alt text](../image/6주차/48강-라인.png)


- 테두리와 라인은 데이터를 기준으로 구분
- 테두리 서식 : 뷰에서 테이블, 패널, 셀 및, 머리글을 둘러싸는 라인의 서식을 설정,
- 라인서식은 뷰에서 표시된 데이터 축에 대한 모양을 설정



## 49강. 대시보드패널

<!-- 대시보드패널 강의에서 알게 된 점을 적어주세요. -->

![alt text](../image/6주차/49강.png)

워크시트를 기반으로 구성할 수 있고, 이미지, 웹사이트, 텍스트등을 첨부할 수 있음.

## 50. 대시보드 구성방식

<!-- 알게 된 점을 적고, 아래 질문에 답해보세요 :) -->

> **🧞‍♀️ 부동과 바둑판식 방식을 차이를 중점으로 기술해보세요**
```
⚫바둑판 
: 개체 추가시, 격자무늬 구조의 특정위치에만 개체들을 구성할 수 있음.

-> 개체 추가 시, 다른 개체들의 크기에 영향을 줌

⚫부동 
: 개체를 자유롭게 배치할 수 있으며, 사용자가 원하는대로 개체를 drag & drop 할 수 있음.

-> 개체 추가시, 다른 개체의 크기나 모양에 영향을 주지 않음.

Shift + drag&drop -> 부동식으로 추가 
```
```
❗TIP❗

<대시보드의 크기가 자주 바뀐다면>, 

"바둑판"을 추천.

- 대시보드의 크기가 비율에 따라 유사한 형식을 유지하기 때문.

---------------------------

<대시보드의 크기가 자주 변경되지 않고, 그래프 내에 빈 공간이 많은 경우>, 

"부동 개체" 를 사용해 빈공간을 채울 수 있음.
```

## 51. 대시보드 컨테이너
**✅ 컨테이너**

**대시보드 개체들과 워크시트들을 그룹화하고 구성할 수 있는 공간**

1) 가로 

    : 내부의 개체들을 ***수평 공간***으로 배열할 때 사용

![alt text](../image/6주차/51강-가로컨테이너.png)


개체가 서로 수평적으로 위치해있으므로, 가로 컨테이너 사용.

2) 세로
    : 내부의 개체들을 ***수직 공간***으로 배열할 때 사용

![alt text](../image/6주차/51강-세로컨테이너.png)

라인그래프와 막대그래프는 서로 수직적으로 배치 => 세로 컨테이너 활용


✅ 컨테이너가 제대로 배치되었는지 확인하기 위해서는 '레이아웃'탭에서 "항목 계층"항목에서 확인 가능

✅ 컨테이너의 '높이 편집' 옵션에서 배너의 사이즈 변경 가능,
   - 드롭다운 메뉴에 나타나지 않으면, 처음에 배치한 세로 컨테이너가 없거나, 가로 컨테이너가 세로 컨테이너 내에 배치되지 않은 것 

## 52. 레이아웃 패널

대시보드의 디자인을 변경할 경우, 몇 가지 인터페이스를 통해 변경할 수 있음.

그 중 하나 : 레이아웃 탭
- 대시보드의 개체 속성을 변경할 수 있음.
- 그래프 클릭 > 레이아웃 tab > 옵션 변경
```
✅ 옵션 설명

* 그래프의 제목은 워크시트의 제목으로 기본 설정 -> 숨김가능

* 개체를 부동 개체로 변경 가능. 
(하지만 부동옵션 해제시, 제자리로 돌아가지 않음.)

* 위치&크기 옵션
: 개체의 위치와 크기를 픽셀단위로 변경가능(부동 개체만 가능)

* 여백 옵션
: 배경 색상을 대시보드 모두에 지정하고 싶을 때,

* 바깥쪽 여백
: 선택된 개체의 모서리와 컨테이너의 테두리 사이의 공간을 변경할 수 있음

* 항목 계층
: 대시보드에 있는 컨테이너와 개체를 볼 수 있음.

```


## 53. 필터 동작

<!-- 필터 동작에 대해 알게 된 점을 적어주세요 -->

차트 클릭 > 드롭다운 메뉴에서 '필터' 선택

❗'국가 선택'과 같이 선택 옵션이 많은 경우에는, 대시보드 동작을 사용하는 것이 더 직관적일 수 있음.

### 대시보드 동작

: 사용자는 대시보드의 차트와 직접 상호작용할 수 있음.

1. 대시보드 tab > '동작'

    : 통합 문서에 있는 대시보드 동작을 확인할 수 있음.

**워크시트와 연계되지 않은 경우**

![alt text](../image/6주차/53강-동작.png)

2. 이 시트 옵션 선택 > 원하는 동작 추가

![alt text](../image/6주차/53강-필터동작.png)

3. 필터 동작을 추가할 시트 설정 & 실행 조건 확인

![alt text](../image/6주차/53강-필터동작2.png)

4. 동작 실행시, 변경할 워크시트 선정

![alt text](../image/6주차/53강-필터동작3.png)

 
번외) 다른 방법

1. 차트를 선택 > "필터로 사용" 기호 선택 > 대시보드 동작 리스트에 동작 추가됨.

2. 해당 동작의 편집화면에서 위의 방법과 동일하게 편집.

## 54. 대시보드 하이라이터 동작

<!-- 하이라이터에 대해 알게 된 점을 적어주세요 -->


## 55. 대시보드 URL

<!-- URL에 대해 알게 된 점을 적어주세요 -->


## 56. 대시보드 시트에 이동 동작

<!-- 대시보드 시트에 이동에 대해 알게 된 점을 적어주세요!-->

## 57. 매개변수 변경 동작

<!-- 매개변수 변경 동작에 대해 알게 된 점을 적어주세요!-->

## 문제

오늘은 별도의 문제가 없습니다. 

![1](../study/img/3rd%20study/1688556627184.png)

![1](../study/img/3rd%20study/Global%20SuperStore%20Dashboard.png)

![2](../study/img/3rd%20study/images.jpeg)
![2](../study/img/3rd%20study/maxresdefault.jpg)

여러 대시보드를 참고하시어, superstore 데이터를 사용해 나만의 대시보드를 제작해주세요.

**단, 워크시트 3개 이상의 그래프를 표시해야 하며 각 시트 간 상호작용성 필터 or 하이라이트 동작은 꼭 추가되어야 합니다**

어떤 부분에 가중을 두었는지, 어떤 사용자 편의성을 고려하였는지에 대한 설명이 필요합니다.
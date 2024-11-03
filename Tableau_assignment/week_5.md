# Fifth Study Week

- 39강: [LOD](#39강-lod)

- 40강: [EXCLUDE](#40-lod-exclude)

- 41강: [INCLUDE](#41-lod-include)

- 42강 : [매개변수](#42-매개변수)

- 43강 : [매개변수 실습](#43-매개변수-실습) 
![링크](https://youtu.be/GJvB8hBqeE8?si=3jIj1iymZHZ7mBam)

- 44강: [매개변수 실습](#44-매개변수-실습)

- 45강: [마크카드](#45-워크시트-마크카드)

- 46강: [서식계층](#46-서식-계층)

- 47강: [워크시트](#47-워크시트-서식)

- [문제1](#문제-1)

- [문제2](#문제-2)

## Study Schedule

| 강의 범위     | 강의 이수 여부 | 링크                                                                                                        |
|--------------|---------|-----------------------------------------------------------------------------------------------------------|
| 1~9강        |  ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=84)       |
| 10~19강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=75)       |
| 20~29강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=65)       |
| 30~38강      | ✅      | [링크](https://www.youtube.com/watch?v=e6J0Ljd6h44&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=55)       |
| 39~47강      | ✅      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=45)       |
| 48~59강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=35)       |
| 60~69강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=25)       |
| 70~79강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=15)       |
| 80~89강      | 🍽️      | [링크](https://www.youtube.com/watch?v=AXkaUrJs-Ko&list=PL87tgIIryGsa5vdz6MsaOEF8PK-YqK3fz&index=5)        |


<!-- 여기까진 그대로 둬 주세요-->

> **🧞‍♀️ 오늘의 스터디는 지니와 함께합니다.**


## 39강. LOD
**LOD : Level Of Detail; 뷰의 세부수준**

ㄴ> 현재의 뷰에는 영향을 받지 않고, 계산할 수준을 세부적으로 제어 가능

### ✅[FIXED]
: 현재 뷰와 상관없이 원하는 차원에서 계산 가능

1) FIXED에서 설정한 차원이 뷰에 포함되어있을 때 
![alt text](<../image/5주차/각 지역의 국가별 매출.png>)
    - 현재 뷰 : 각 지역의 국가별 매출

    ![alt text](../image/5주차/LOD-FIXED.png)
    
    - fixed함수로 계산된 필드 만들어서 지역별 매출 표시 가능(중괄호 활용)
    - 계산식 작성 시 여러 개의 차원을 기준으로 할 때, 각 차원들을(,)로 구분

   ![alt text](<../image/5주차/지역별 매출.png>)
    ![alt text](../image/5주차/지역별매출(FIXED).png)
    
    - 국가/지역별 매출이아니라 FIXED에 설정한 [지역]의 값으로 세부값 표시

2) FIXED에서 설정한 차원이 뷰에 포함되어있지 않을 때,

![](<../image/5주차/전체 데이터 (FIXED).png>)

- LOD표현식에서 차원을 입력하지 않으면 전체 데이터 기반으로 계산
- 전체 데이터를 기반으로 구성비율 계산할 수 있음

## 40. LOD EXCLUDE
**: *현재 뷰*에서 특정 차원을 제외하여 계산할 때 사용**

![alt text](<../image/5주차/LOD EXCLUDE-1.png>)
지금 화면은 하위 범주별 매출이 나와있음.

하지만 범주별 매출이 보고싶다면 FIXED 혹은 EXLUDE를 사용해야함

- FIXED 계산식
![](<../image/5주차/LOD EXCLUDE-2.png>)

- EXCLUDE 계산식
![alt text](<../image/5주차/LOD EXCLUDE-3.png>)
    - 하위범주를 'EXCLUDE' 하지만 '제조업체' 차원이 하위범주보다 세부수준이 낮아서 제조업체를 기준으로 값을 표시함.
<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적고, 아래 두 질문에 답해보세요 :) -->

> **🧞‍♀️ FIXED와 EXCLUDE을 사용하는 경우의 차이가 무엇인가요?**

```
*FIXED: 현재 뷰와 상관없이 특정 차원만을 사용해서 값을 계산 -> 필터의 영향 X
=> 고정된 차원의 값

*EXCLUDE: 뷰의 차원을 따라 계산하기 때문에 FILTER나 세부수준에 따라 값이 달라진다
```

**악세사리를 기준으로 다른 제품들의 매출을 비교해보자**
![alt text](<../image/5주차/LOD EXCLUDE-4.png>)

1. 악세사리의 매출을 계산하는 필드 생성
![alt text](<../image/5주차/LOD EXCLUDE-5.png>)

2. 더블클릭하면 악세사리의 매출값만 표시됨
![alt text](<../image/5주차/LOD EXCLUDE-6.png>)

3. 제품마다 "액세서리"의 매출값을 표시하는 필드를 만들기 위해서 계산된 필드 생성
![alt text](<../image/5주차/LOD EXCLUDE-7.png>)
: 해당 함수가 하위 범주 차원을 무시하고 액세서리의 매출 값만 반환

4. 적용
![alt text](<../image/5주차/LOD EXCLUDE-8.png>)

5. 각 제품별 매출과 악세사리의 매출의 차이를 나타내는 필드 생성
![alt text](<../image/5주차/LOD EXCLUDE-9.png>)
**[적용 +  CTRL해서 색상에 드래그&드랍한 모습]**
![alt text](<../image/5주차/LOD EXCLUDE-10.png>)
->모든 제품들의 매출이 악세사리 매출을 기준으로 얼마나 차이가 나는지 한 눈으로 확인 가능

(파란색: 악세사리보다 높은 매출/주황색: 악세사리보다 낮은 매출)



> **🧞‍♀️ 왜 ATTR 함수를 
사용하나요?**

```
해당 값이 단일값인지 확인하기 위해서
단일 값이면 그 값을 반환하고, 그렇지 않으면 *나 NULL을 반환한다.
```


## 41. LOD INCLUDE
**: 현재 뷰에서 특정 차원을 추가해서 계산하는 방삭**

- 차원 필터에 따라 값이 변경함

**✅각 도시의 고객당 평균 매출**





> **🧞‍♀️ 그렇다면 어떤 경우에 각 표현식을 사용하나요? 예시와 함께 적어보아요**


```
여기에 답을 적어주세요!
```

## 42. 매개변수

<!-- 매개변수에 대해 알게 된 점을 적어주세요 -->

> **🧞‍♀️ 집합에도 매개변수를 적용할 수 있나요? 시도해봅시다**


## 43. 매개변수 실습
<!-- 영상 묶음에 포함되지 않아 찾기 어려우실까 링크를 아래에 첨부하겠습니다. 수강 후 삭제해주세요-->

https://www.youtube.com/watch?v=GJvB8hBqeE8

## 44. 매개변수 실습

<!-- 매개변수에 대해 알게 된 점을 적어주세요 -->

## 45. 워크시트 마크카드

<!-- 마크카드에 대해 알게 된 점을 적어주세요 -->


## 46. 서식 계층

<!-- 서식계층에 대해 알게 된 점을 적어주세요 -->

> **🧞‍♀️ 서식계층을 일반적인 것에서 구체적인 것 순서로 기입해보세요**


```
여기에 답을 적어주세요!
```


## 47. 워크시트 서식

<!-- 워크시트 서식에 대해 알게 된 점을 적어주세요!-->



## 문제 리스트



## 문제 1.

```
가장 많이 주문한 사람들은 물건 배송을 빨리 받았을까요?
조건을 준수하여 아래 이미지를 만들어봆시다.
1) 국가/지역별(이하 '나라'로 통칭), 범주별로 배송일자가 다를 수 있으니 먼저, 나라별/범주별로 평균 배송일자를 설정한 뒤,
2) 각 나라에서 가장 많이 주문한 사람의 이름을 첫 번째 열,
3) 그 사람이 주문한 제품 이름을 2번째 열,
4) 각 상품이 배송까지 걸린 날 수를 표현하고
5) 그리고 만약 배송이 각 나라/범주별 평균보다 빨랐다면 '빠름', 같다면 '평균', 느리다면 '느림' 으로 print 해주세요. 
```

![이미지주소](https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/2nd%20study/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202024-08-13%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2010.12.36.png?raw=true)

<!-- 여기까지 오는 과정 중 알게 된 점을 기입하고, 결과는 시트 명을 본인 이름으로 바꾸어 표시해주세요.-->

## 문제 2.

```
채원이는 태블로를 쓰실 수 없는 상사분께 보고하기 위한 대시보드를 만들고 싶어요. 

제품 중분류별로 구분하되 매개변수로써 수익, 매출, 수량을 입력하면 저절로 각각 지표에 해당하는 그래프로 바뀌도록 설계하고자 해요.

 어떤 값이 각 지표의 평균보다 낮은 값을 갖고 있다면 색깔을 주황색으로, 그것보다 높다면 파란색으로 표시하고 싶어요. 그 평균값은 각 지표별로 달라야 해요.
```

![example](https://github.com/yousrchive/BUSINESS-INTELLIGENCE-TABLEAU/blob/main/study/img/2nd%20study/%E1%84%83%E1%85%A1%E1%84%8B%E1%85%AE%E1%86%AB%E1%84%85%E1%85%A9%E1%84%83%E1%85%B3.png?raw=true)

<!-- 예시 사진은 지워주세요-->
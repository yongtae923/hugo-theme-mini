+++
author = "김용태"
title = "여러가지 확률분포(2) - Hypergeometric distribution(초기하 분포)"
date = "2023-04-18"
tags = ["수학"]
draft = false
+++

어떤 공장에서 제품이 하루에 100개씩 만들어져 나온다.

그런데 그 제품들 중에서 불량품이 항상 5개씩 만들어진다고 하자. (그럼 정상품은 95개가 나온다.)

하루에 나온 제품들 중 10개를 잡아 검사했을 때 발견된 불량품의 개수가 3개일 확률은 얼마일까?

---

위 문제를 풀 때 사용할 수 있는 확률 분포(probability distribution)은 초기하 분포(hypergeometric distribution)이다.

초기하 분포의 특징은 이항 분포(binomial distribution)와 비슷하다.

이항 분포는 베르누이 시행(Bernoulli trial)을 반복할 때, 이전 시행이 다음 시행의 결과에 영향을 주지 않는다.

그러나 초기하 분포에서는 시행을 하면 다음 시행에서 결과값이 바뀐다.

쉽게 위의 예시를 이용해서 설명하면, 베르누이 시행은 제품 검사와 같다.

이항 분포는 제품 검사를 할 때, 한 제품을 골라 검사하고 다시 돌려놓은 뒤 다시 전체에서 하나를 골라 검사한다.

따라서 제품 검사를 한 번 했다고 해서 다음 검사에서 불량품이 걸릴 확률이 바뀌지 않는다.

그러나 초기하 분포는 한 제품을 골라 검사하고 난 뒤에 그 제품을 배제한 나머지 중에서 다음 검사할 제품을 고른다.

따라서 제품 검사를 한 번 하면 그 결과에 따라 다음 검사할 나머지 제품들 중에서 불량품이 나올 확률이 달라진다.

---

이제 초기하 분포를 사용해보자.

N개의 제품 중 불량품은 k개가 들어있고, N개 제품 중 n개를 골라 검사할 때 나오는 불량품의 개수 x를 초기하확률변수(hypergeometric random variable)이라 한다.

이 초기하확률변수를 결과값으로 하여 확률을 도출하는 함수가 초기하확률분포이다.

표기는 다음과 같이 한다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681628849853/d3b07fc6-5b7d-46e6-90a4-87902a09836e.png)

h는 함수이름(hypergeometric의 앞글자), N은 전체 제품수, x는 결과값(불량품검출수), n은 시행횟수(검사횟수), k는 불량품의 개수이다.

이제 문제의 변수를 대입하자.

100개의 제품 중 불량품은 5개, 전체 제품들 중에서 10개를 골라 검사했을 때 3개가 불량품일 확률을 구한다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681628889300/1a13d38f-84af-4415-858c-8621b610c9d9.png)

---

초기하확률변수의 평균(mean)과 분산(variance)는 다음과 같다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681628901121/adf499fb-8116-4524-99bd-cfa121e464bb.png)

출처

Walpole, R. E., & Myers, R. H. (2016). *Probability and statistics for engineers and scientists*. New York: Macmillan.
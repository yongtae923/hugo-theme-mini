+++
author = "김용태"
title = "여러가지 확률분포(1) - Binomial distribution(이항 분포)"
date = "2020-02-29"
tags = ["수학", "확률"]
draft = false
+++

확률 분포란 어떤 상황에서 결과값이 나올 확률을 나타내는 함수를 나타낸다.

> 함수
> 
> 정의역 -&gt; 치역
> 
> 결과값 -&gt; 확률

대충 위와 같은 관계로 나타낼 수 있다. 확률 분포에 대해서는 나중에 다시 설명하겠다.

---

그 중 대표적인 확률 분포(probability distribution)인 이항 분포(binomial distribution)을 알아보자.

주사위를 한 번 던졌을 때, 1이 나오면 성공이라고 치자.
처음 주사위를 던졌을 때, 성공할 확률은 1/6이다.
두번째로 주사위를 던졌을 때, 다시 성공할 확률은 1/6이다.
두번째에서 성공할 확률은 첫번째의 결과가 1인지 아닌지와 관계없이 1/6이다.
주사위를 계속해서 던졌을 때, 성공한 횟수를 X라 하자.

위와 같은 예시에서 우리는 주사위를 10번 던졌을 때 5번 성공할 확률을 구하고 싶다고 하자.

위 상황의 특징은 다음과 같다.

1. 같은 시행(주사위를 던지는 것)을 반복한다.
    
2. 각각의 시행에서 결과는 성공(1이 나오는 것)과 실패 중 하나이다.
    
3. 각각의 시행에서 성공할 확률 p(1/6)는 일정하다.
    
4. 각각의 시행은 독립적이다. = 이전에 나온 시행 결과에 따라 이후 시행의 확률이 바뀌지 않는다.
    

우리는 이러한 경우에 이항 분포(binomial distribution)을 쓸 수 있다.

참고로 이 상황은 베르누이 과정(Bernoulli process)라고 하며, 각각의 시행은 베르누이 시행(Bernoulli trial)이라고 한다.

---

이항 분포를 쓸 수 있다고 했는데 어떻게 쓰는지 보자.

n번의 시행에서 성공한 횟수 X개는 이항확률변수(binomial random variable)이라 한다.

이 이항확률변수를 결과값으로 하여 확률을 도출하는 함수가 이항 분포(binomial distribution)이다.

표기는 다음과 같이 한다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681461486165/50578605-fcfe-409e-8901-b318fdefd4f3.png)


b는 함수이름(binomial의 앞글자), x는 결과값(성공횟수), n은 시행횟수, p는 각 시행에서 성공확률이다.

그렇다면 이항 분포를 구해보자.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681461502431/170f0712-e4a5-440c-a6ae-0a4e9b0441e3.png)

베르누이가 대신 구해줬다.

q는 1-p이고, 그 밖에 모르는 건 순열과 조합을 검색하자.

이제 처음 들었던 주사위 예시를 풀어보자.

문제에서 시행 횟수 n은 10, 성공 횟수 x는 5, 성공 확률 p는 1/6이다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681461520753/532ce3b0-dc4b-44c9-b7ab-a9082e9d2b03.png)

주사위 10번 던져서 정확히 5번이 성공할 확률이 나왔다.

숫자가 더러울 때는 계산기나 울프럼알파를 쓰자.

출처

Walpole, R. E., & Myers, R. H. (2016). Probability and statistics for engineers and scientists. New York: Macmillan.

---

이 게시글은 2020년 2월 29일 [네이버 블로그](https://blog.naver.com/yongtae923/221830514483)에 게시되었습니다.
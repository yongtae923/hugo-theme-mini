+++
author = "김용태"
title = "미분방정식 푸는법 요약"
date = "2020-10-15"
tags = ["수학"]
draft = false
+++

곧 시험이니까 미분방정식(Differential Equation) 푸는 법을 정리한다.

유도 과정은 적지 않았으며 답만 구할 수 있으니 과정은 스스로 공부하면서 파악한다.

## 1\. Reduction of Order

미분방정식이 homogeneous하고 이차항이 최고차항이며 두 해 중 하나를 알고 있다면 다른 해를 구할 수 있다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691820371/50dea1e5-19f2-4c7a-b701-e6e239a7c821.png)

위 식의 한 해가 y1이면 다른 해 y2를 구할 수 있다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691830529/2b9dde29-aad9-479f-8039-b52f394d35de.png)

## 2\. Constant Coefficients

위와 비슷한 ay''+by'+cy=0 식에서 y=me^x를 대입하면 am^2+bm+c=0 이 된다.

이 이차식의 두 해가 서로 다른 실수 m1, m2라면 미방의 일반해는 y=c1\*e^(m1x)+c2\*e^(m2x)

두 해가 서로 같은 실수 m이면 일반해는 y=c1\*e^(mx)+c2\*e^(mx)\*x

두 해가 두 실수 k,m에 대해 m+ki와 m-ki라면 일반해는 y=e^(mx)\*(c1\*cos(kx)+c2\*sin(kx))

## 3\. Undetermined Coefficients

미방이 non-homgeneous 하다면 일반해에 특수해를 더해야 한다.

ay''+by'+cy=g(x)의 일반해는 g(x)를 0으로 가정하고 2번과 같이 구한다.

그 다음 특수해를 구하려면 g(x)의 형태에 따라 상수 A, B, C, ...를 가정하고 특수해(yp)의 꼴을 만든다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691838242/a44fae48-bd56-4f65-8ed4-19af82a242c2.png)

만약 일반해와 특수해의 꼴이 같은 항이 있으면 특수해의 그 항에 x^n을 곱해준다.

그 후에 상수 A, B, C, ...를 포함한 특수해를 구하려는 미방에 대입하여 각 상수를 알아낸다.

미방을 푼 결과는 일반해와 특수해의 합이다.

## 4\. Variation of Parameters

이 방법은 3번으로 푸는 도중 도저히 특수해의 꼴을 알 수 없을 때 쓰는 방법이다.

ay''+by'+cy=g(x) 를 a로 나누어서 y''+P(x)y'+Q(x)y=f(x) 가 되었다고 한다.

2번의 방법으로 일반해를 y=c1\*y1+c2\*y2 로 구한다.

Wronskian W=y1\*y2' - y2\*y1'

u1'(x) = - y2\*f(x) / W 이고 u2'(x) = y1\*f(x) / W 이다. u1'과 u2'를 각각 적분한다.

미방의 답은 y = u1\*y1+u2\*y2 이다.

## 5\. Cauchy-Euler Equation

코시-오일러 방정식은 아래처럼 생긴 식이다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691845218/ead536d3-ced1-4d36-aba8-c901f9b191f3.png)

2차식이면 y=x^m을 대입해서 a\*m\*(m-1)\*b\*m+c=0 인 auxiliary equation을 만들 수 있다.

이 식을 풀어서 나온 두 해가 서로 다른 실수 m1, m2면 미방의 일반해는 y = c1\*x^m1 + c2\*x^m2

두 해가 서로 같은 실수 m이면 일반해는 y = c1\*x^m + c2\*x^m\*lnx

두 해가 두 실수 k,m에 대해 m+ki, m-ki이면 일반해는 y = x^m\*(c1\*cos(k\*lnx)+c2\*sin(k\*lnx))

## 6. Reduction of Order (Nonlinear)

비선형 미방은 깔끔하지 못한 식인 경우가 많은데, 간단하게 dependent y나 x가 없을 경우부터 본다.

F(x, y',y'')=0이나 F(y,y',y'')=0 같은 식일 때는 u=y', u'=y''을 대입하면 쉽게 풀리는 경우가 있다.

그래도 안 되면 테일러 급수를 대입한다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691856173/a840f7a9-2b49-4854-b759-63ffd6da9f57.png)

y를 이렇게 가정하고 미분해서 미방에 대입하면 테일러 급수 형태의 답이 나올 것이다.

## 7. Green's Function

4번을 응용하면 아래의 Green's Function으로 특수해를 구할 수 있다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691862292/afc6da2c-c3e0-4b50-9682-b5441384c59d.png)

일반해 yc를 구하고 거기에 초기값을 대입하여 yh를 구한 뒤 Green's Function으로 구한 특수해를 더할 수 있다.

---

다시 적지만 답을 구하는 것보다 풀이 과정을 아는 것이 더 중요하다.

이 글은 시간이 촉박할 때에 답을 얻어내는 것이 전부다.

시간이 충분할 경우에는 각각의 공식을 증명해보면 많은 도움을 줄 것이다.

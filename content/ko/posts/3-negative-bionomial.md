+++
author = "김용태"
title = "여러가지 확률분포(3) - Negative binomial distribution(음이항 분포)"
date = "2023-04-18"
tags = ["수학"]
draft = false
+++

우리는 이항 분포가 베르누이 시행에서 몇 번의 시행이 나올 확률을 구하는 확률변수임을 배웠다.

그렇다면 이름이 음(negative)이 붙은 이 음이항 분포는 무엇이 다를까?



음이항 분포는 성공할 때까지의 시행 횟수에 더 관심을 가진다.

즉, 이항 분포가 주사위를 다 던져놓고나서 몇 번 성공했나... 세면서 성공횟수에 관심을 가진다면

음이항 분포는 한 번 던질 때마다 이번에는 성공했나...? 이러면서 보다가,

어느 순간 몇 번의 성공횟수가 쌓이면 거기서 멈추고 지금까지 몇 번 던졌는지 물으며 시행횟수에 관심을 가지는 것이다.

---

성공확률은 p이고, k번의 성공횟수가 쌓일 때까지 시행한 횟수가 x일 확률은 다음과 같이 표현된다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681690771091/271a5d52-451c-4067-888b-05467c958728.png)

예를 들어 주사위에서 한 번 던졌을 때, 1이 나올 확률은 1/6이고, 그걸 성공이라 하자.

던지기를 계속 반복하면서 성공횟수를 세다가 5번째 성공이 나왔을 때, 그 시행이 전체에서 12번째일 확률을 구해보자.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681690780953/640cd5a4-a4d5-4a77-a65d-3b8f26996b15.png)

더러운 계산은 울프럼알파에게 맡기자.



출처

Walpole, R. E., & Myers, R. H. (2016). *Probability and statistics for engineers and scientists*. New York: Macmillan.
+++
author = "김용태"
title = "여러가지 확률분포(4) - Geometric distribution(기하 분포)"
date = "2020-03-14"
tags = ["수학", "확률"]
draft = false
+++

기하 분포(geometric distribution)은 음이항 분포(negative binomial distribution)과 매우 비슷하다.



음이항 분포는 시행을 계속하며 k번 성공했을 때 그때까지의 시행횟수에 관심을 가진다.

기하 분포는 시행을 계속하며 첫번째 성공했을 때 그때까지의 시행횟수에 관심을 가진다.



즉, 기하 분포는 음이항 분포에서 변수 k에 1을 대입한 경우와 같다.

---

성공확률은 p이고, 실패 확률은 1-p=q이며, 첫번째 성공할 때 음이항 분포는 기하 분포와 같다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691135715/0ba0d20a-45b0-484f-9601-9c2919eb9a36.png)

g는 기하 분포(geometric distribution)의 앞글자에서 따왔다.

---

예를 들어 주사위를 성공이 나올 때까지 던지다가 10번째에서 첫번째 성공이 나올 확률을 구해보자.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691144685/c66e8f8f-aec7-4b51-a527-a8c4387ea56d.png)

실패 9번 나올 확률에 성공 1번 나올 확률을 순열로 구한 것과 같음을 관찰할 수 있다.

---

기하 분포의 평균과 분산은 다음과 같다.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681691150287/1f70e81f-3e2e-4f0f-89c7-489d79f7e562.png)

출처

Walpole, R. E., & Myers, R. H. (2016). *Probability and statistics for engineers and scientists*. New York: Macmillan.
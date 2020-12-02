#  matplotlib + seaborn 그래프 그리기

![zz](https://matplotlib.org/3.3.3/_static/logo2_compressed.svg) </br></br>

matplotlib 과 seaborn에서 제공하는 docs를 가시면 더욱더 자세하게 해당 내용을 익힐수 있다. </br>
<https://matplotlib.org/> <--matplotlib Docs<br>
<https://seaborn.pydata.org/index.html> <-- seaborn Docs

__글쓰기 앞서 다양한 그래프를 그리면서 겪었던 상황중 하나 항상 나의 VERSION 확인 !!!__

도움을 주신 분 : Jaehyun Lee(aka. Pega) 님 감사합니다. <br>
<https://jehyunlee.github.io/> <-- 페가님 블로그에서 많은부분을 배울수있었다. <br><br>

커뮤니티 활동을 하다보면 그래프를 어떻게 그려야할지 힘들어하시는 개발자분들을 많이 경험했다.<br>
간단히 말해 그래프에 대한 나의 생각은 내가 Tensorflow KR에 적었던 댓글으로 요약된다<br>
<img width="187" alt="aaa" src="https://user-images.githubusercontent.com/41941627/100684505-d0367f00-33bd-11eb-852d-66563331ae40.png">


# Introduction
우선 데이터분석의 파이썬 3대장(?) 이라고 불리는것들엔 무엇이 있을까 ?<br>
이 글을 본사람들 중 파이썬으로 데이터를 다뤄본사람이라면 Pandas, Numpy, Matplotlib이라고 대답할 것이다.<br>
위에 언급했던 3개의 라이브러리중 앞에 2개는 전처리 과정을 필사하고 자주겪다보면 자연스레 조금씩 알아간다고 느낀다.<br>
하지만 그래프는 나에게는 필사를 하면 이해는되지만 막상 내가 그래프를 그리려하면 기본적인 그래프밖에 못그리는게 현실이다.<br>
사실 복잡한 그래프가 어려워 BI툴들을 사용하여 PPT를 만든 기술력이 터무니없는(?) 경험을 하기도했다.<br>
따라서 하나씩 현재 내가 마주하는 데이터들로 하여금 그래프를 그려나가보려고 한다.<br>


# Table of content
 
1. 그래프 그리기
2. 그래프 그리기 실습
3. 계속적으로 추가예정...


# what is matplotlib ?

matplotlib은 다양한 데이터를 많은 방법으로 도식화 할 수 있도록 하는 파이썬 라이브러리로써, 우리는 matplotlib의 pyplot을 이용하게 된다.<br>
이는 mathworks에서 개발한 매트랩(MATLAB)과 비슷한 형태를 가지고 있다.<br>
matplotlib을 이용하면 우리가 이전에 알아본 numpy나 pandas에서 사용되는 자료구조를 쉽게 시각화 할 수 있다.<br>
matplotlib을 사용하기 위해서는 먼저 matplotlib을 설치하고 아래와 같이 import를 해주어야 합니다.<br>
mat + plot + lib 세가지로 분리해  'Mat 이라는 그래프 그려주는 라이브러리' 정도로 쉽게 기억하자 . <br>

<br><br>
import matplotlib
<br>
import matplotlib.pyplot as plt
<br>
이런식으로 쓰여진다.
# What is seaborn ?

Seaborn은 기본적으로 matplotlib를 베이스(밑단)으로 삼고 최상위 단에서 연산을 하는 모양이다. 
pandas 데이터 구조를 사용하여 입출력을 받아 연산을 합니다. matplotlib을 기반으로 했다는 건 matplotlib에서 '추가적으로 사용가능한 확장판' 정도로 이해하면 좋을 것 같다.<br>

# 그럼 레퍼지토리의 코드들로 실제 실습을 해보자.


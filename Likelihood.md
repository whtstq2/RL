---


---

<h1 id="likelihood">Likelihood</h1>
<p>어떤 표본에서 특정한 값의 집합인 확률변수를 고정된 모집단 모수θ의 결합 확률밀도함수(joint probability  density  function)로 표현한 것이다.</p>
<h2 id="간단히">간단히</h2>
<p>우도 = likelihood<br>
likelihood란 간단히 말해서 판단 척도로 사용되는 도구이다.<br>
우리가 흔히 보는 Maximum likelihood는 이 likelihood가 가장 높은 것을 택한다는 판단 기준이다.</p>
<p>베이스 가설이 있다고 치자 그런데 새로운 증거가 나타났다. 그래서 그 증거를 바탕으로 새 가설로 바꿨다. 그런데 과연 이 가설이 이전의 가설보다 나은 것인가?</p>
<p>가설의 불확실성을 평가하기 위해 흔히 사용되는 Bayes’ Theory에서는 이전 확률에 새로운 사건을 더해 다음 확률을 만든다. 그런데 이전 확률 즉, 베이스 가설에는 자의성이 들어갈 수 밖에 없는데 (모든 가설의 시작은 휴리스틱할 수 밖에 없다) 아예 배제 할 수는 없겠지만 최대한 줄이기 위해 likelihood를 사용한다.</p>
<p>Likelihood = 관찰치를 얻을 확률을 최대화하는 모수의 값</p>
<p>• <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f17.gif)<![endif]> 의 함수가  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f19.gif)<![endif]> 로 주어질 때,

1) <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f1b.gif)<![endif]> 의 log likelihood function은  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f1d.gif)<![endif]> 이며,

<![if !supportEmptyParas]> <![endif]>

￭ score function

2) 따라서 Score function은 다음과 같은 형태로 주어진다.

<![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f1f.gif)<![endif]>

3) 이 때, <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f21.gif)<![endif]> 의 MLE인  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f23.gif)<![endif]> 는  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f25.gif)<![endif]> 을 만족시킨다.

<![if !supportEmptyParas]> <![endif]>

￭ observed information

4) 한편, <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f27.gif)<![endif]> 부근에서 score function은 approximately linear하므로 Taylor's expansion을 이용하여, 다음과 같은 식을 얻는다.

<![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f29.gif)<![endif]>

5) 위 식에서 <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f2b.gif)<![endif]> 인데, 이 값이 음이기 때문에 이를 고려하여  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f2d.gif)<![endif]> 로 표현하고, 이를 observed information이라 하며  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f2f.gif)<![endif]> 로 쓴다.

6) 한편, <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f31.gif)<![endif]> 이기 때문에 4)의 식은  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f33.gif)<![endif]> 이 된다.

<![if !supportEmptyParas]> <![endif]>

￭ <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f35.gif)<![endif]>

7) <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f37.gif)<![endif]> 의 추정치  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f39.gif)<![endif]> 의 frequency에 관한 성질을 추정함에 있어서,  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f3b.gif)<![endif]> 를 이용하는 것이 가장 좋은데, likelihood접근법에서 이 함수[ <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f3d.gif)<![endif]> ]에 대한 가정은 data( <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f3f.gif)<![endif]> )를 고정된 것으로 보고,  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f41.gif)<![endif]> 를 변화하는 것으로 보는 것이다.

∙ frequency접근법에서는 data( <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f43.gif)<![endif]> )를 변화하는 것으로 보고,  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f45.gif)<![endif]> 를 고정된 것으로 본다. 즉, frequency접근법에서는  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f47.gif)<![endif]> 및  <![if !vml]>![](file:///C:\Users\whtstq2\AppData\Local\Temp\DRW00003df81f49.gif)<![endif]> 가 random variable이 된다.

<![if !supportEmptyParas]> <![endif]></p>
<h2 id="likelihood-ratio">Likelihood ratio</h2>
<p>likelihood의 비<br>
<img src="http://www.aistudy.com/math/images/likelihood_htm_eqn17.gif" alt=""></p>
<h2 id="여기서-잠시">여기서 잠시,</h2>
<p>여기서 잠시, 확률은 <a href="https://terms.naver.com/entry.nhn?docId=393305&amp;ref=y">정문제</a>와 관련된 반면 likelihood은 <a href="https://terms.naver.com/entry.nhn?docId=395229&amp;ref=y">역문제</a>와 관련되어 있다. 확률은 무엇무엇 조건이 있을 때 사건이 있을 가능성이라면 likelihood는 사건이 일어났을 때 어떤 가설에 의한 것일 가능성인 것이다.</p>
<h2 id="log-likelihood">Log Likelihood</h2>
<p>Log Likelihood는 likelihood 계산을 쉽게 하기 위함이다.<br>
위에 Likelihood ratio에 log를 취하면 log (a/b) = log a - log b 가 되어서 단순 뺄셈만 하면 된다.</p>
<h2 id="score-function">Score function</h2>
<p>log likelihood를 미분한 것</p>
<h2 id="잡설">잡설</h2>
<p>앞에서 새 가설로 바꿔가는 과정이 강화학습에서 policy를 업데이트하는 것과 같은거라고 생각해도 좋을 것이다.</p>
<p>출처: <a href="http://www.aistudy.com/math/likelihood.htm">http://www.aistudy.com/math/likelihood.htm</a></p>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYwMzE1ODM3Ml19
-->
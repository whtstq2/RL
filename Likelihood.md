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
<p>> Likelihood = 관찰치를 얻을 확률을 최대화하는 모수의 값</p>
<p>이걸 우리가 배우는 머신러닝의 경우로 대입 해보자면 한 함수가 있다. 여러 파라미터들로 이루어진 함수이다. 그 상황에서 우린 파라미터가 (1,2,3,4,5,6…)일 때 데이터를 가장 잘 표현한다고 생각하고 함수를 만들었다. 그랬을 때</p>
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
eyJoaXN0b3J5IjpbLTcyMDA4MzQ3XX0=
-->
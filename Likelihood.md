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

<h2 id="우앵">조금 자세히</h2>
<p> 최대우도법은 어떤 확률변수에서 표집한 값들을 토대로 그 확률변수의 모수를 구하는 방법이다. 어떤 모수가 주어졌을 때, 원하는 값들이 나올 가능도를 최대로 만드는 모수를 선택하는 방법이다. 점추정 방식에 속한다.

즉, 우리는 절대로 모수를 알 수 없다. 따라서 표본(sample)을 통해서 모집단의 특성인 모수를 파악해야한다. 이 때, 우리가 가정하는 것은 각각의 표본을 추출할 때의 확률밀도함수 혹은 확률질량함수의 양상을 알고 있다는 것이다. (즉, 수학적으로 각 sample을 뽑을 확률밀도함수에 대해서 어떤 양상을 따를지 알고 있을 때 모수를 추정하고자 한다면 최대우도법을 쓸 수 있다.)</p>

<p> 어떤 모수  θθ로 결정되는 확률변수들의 모임  Dθ=(X1,X2,⋯,Xn)Dθ=(X1,X2,⋯,Xn)이 있고  DθDθ의 확률밀도함수나 확률질량함수가  ff이고, 그 확률변수들에서 각각 값  x1,x2,⋯,xnx1,x2,⋯,xn을 얻었을 경우 가능도  L(θ)L(θ)는 다음과 같다.

![](http://bit.ly/2kGjih1)

여기에서 가능도를 최대로 만드는  θθ는

![](http://bit.ly/2kT79AL)

가 된다.

이 때  X1,X2,⋯,XnX1,X2,⋯,Xn이 모두 독립적이고 같은 확률분포를 가지고 있다면  LL은 다음과 같이 표현이 가능하다.

![](http://bit.ly/2kSUVrN)

또한, 로그함수는 단조 증가하므로,  LL에 로그를 씌운 값의 최댓값은 원래 값  θ^θ^와 같고, 이 경우 계산이 비교적 간단해진다.

![](http://bit.ly/2kGawzJ)</p>


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
<p> :  <a href="https://wikidocs.net/7679"> https://wikidocs.net/7679</a></p>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM0NDQxODgyNyw4NTI5NzYzNzEsMTE5Nz
AyNTI3M119
-->
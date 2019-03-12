# Finite Markov Decision Process

유한한 MDP에 대한 챕터이다. 
MDP 문제는 가장 기본적인 문제이다. 
연속으로 결정을 내려야하는 문제이고 action시 즉각적인 reward를 받는게 아닐 수도 있다. 
그래서 즉시 얻는 보상과 나중에 얻게되는 보상의 기준을 정하는게 중요하다. Bandit의 경우엔 각 action마다 true value가 있었다. 하지만 MDP에선 action만이 아니라 state까지 고려하여 true value를 추정한다. 또는 최적의 action을 통해 각 상태의 값 v<sub>*</sub>(s) 을 추정한다. 이 state-dependent quantities 들은 long-term return을 정확히 정하는데 필요하다.

MDP는 수학적으로 이상적인 형태의 RL 문제이다. 앞으로 문제의 수학적인 구조에서 중요한 부분들을 설명할 것이다.
예를 들어 return이나 value function, Bellman Equation 들이다.

## 3.1 

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ0NTk2Mzc1LDI3MTk2ODM0NSwtMTc3MD
Q0Mzc5LC0xMjgxNDAxOTcwLDY4NjQyMDMyMCw3NjAxNjQzNzMs
LTIxNzU4MDMxN119
-->
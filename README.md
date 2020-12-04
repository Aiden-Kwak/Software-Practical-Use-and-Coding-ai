# Software-Practical-Use-and-Coding-ai
deep learning part

#0
Linear Regression, Logistic Regression. <br>
가장 훌륭한 예측선 긋기란 Linear Regression을 쉽게 풀어쓴것. 머신러닝은 제대로 된 선긋기에서 시작된다.<br>
*gradient decent<br> 로지스틱회귀에선 sigmoid function을 조정. 이때도 경사하강법 통해서 a,b구함.<br>
만약 입력값이 추가되어 세개이상의 입력값을 다룬다면 시그모이드가 아니라 softmax function 써야한다.

#1
perceptron: 입력값과 활성화 함수를 사용해 출력값을 다음으로 넘기는 가장 작은 신경망 단위
y=ax+b를 퍼셉트론에 맞춰 뭔가 딥러닝스럽게 표현해보면 a는 가중치(weight), b는 바이어스(bias), y는 입력값(x)와 가중치의 곱을 모두 더한다음 바이어스를 더한 값인 가중합(weighted sum)이다.<br>가중합의 결과를 놓고 1 또는 0을 출력해서 활성화함수(activation function)으로 보낸다. 대표적으로 시그모이드 함수
* 퍼셉트론의 한계: XOR problem <br>
XOR 문제를 해결하기 위해서 2개의 퍼셉트론을 한번에 계산할 수 있어야함.<br>
이를 가능하게 하려면 은닉층(hidden layer)만들면 됨. -> 다중 퍼셉트론// 뭔가 신경망을 닮아서 neural network라 부름.

#2
오차 역전파(back propagation): 신경망 내부의 가중치 수정방법// 경사하강법 확장개념임. <br>
임의의 가중치를 선언하고 결과값을 이용해 오차를 구한뒤 이 오차가 최소인 지점으로 계속 이동해서 조금씩 가중치를 이동시킴<br>
이 오차가 최소가 되는점(미분했을 때 기울기 0지점)을 찾으면 그게 찾고자하는 가중치임.

#2
Sequential 함수는 딥러닝의 구조를 한층 한층 쉽게 쌓아올릴 수 있게함.<br> Sequential 함수 선언 후 케라스의 model.add() 함수 사용해 필요한 층을 차례로 추가하면 됨.<br> 
케라스의 장점 중 하나는 model.add() 함수를 이용해 필요한 만큼의 층을 빠르고 쉽게 쌓을 수 있다는 것.<br>
model.add() 안에는 Dense() 함수가 포함되어 있다. -> 각 층이 각각 어떤 특성을 가질지 옵션을 설정하는 역할.<br>
딥러닝의 구조와 층별 옵션을 정하고 나면 compile()함수를 이용해 이를 실행시킴.<br>
* loss, optimizer, activation<br>
블랙박스를 극복하려면?

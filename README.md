# Software-Practical-Use-and-Coding-ai
deep learning part

#0
Linear Regression, Logistic Regression. <br>
가장 훌륭한 예측선 긋기란 Linear Regression을 쉽게 풀어쓴것. 머신러닝은 제대로 된 선긋기에서 시작된다.<br>
*gradient decent<br> 로지스틱회귀에선 sigmoid function을 조정. 이때도 경사하강법 통해서 a,b구함.<br>
만약 입력값이 추가되어 세개이상의 입력값을 다룬다면 시그모이드가 아니라 softmax function 써야한다.

#1
perceptron

#2
Sequential 함수는 딥러닝의 구조를 한층 한층 쉽게 쌓아올릴 수 있게함.<br> Sequential 함수 선언 후 케라스의 model.add() 함수 사용해 필요한 층을 차례로 추가하면 됨.<br> 
케라스의 장점 중 하나는 model.add() 함수를 이용해 필요한 만큼의 층을 빠르고 쉽게 쌓을 수 있다는 것.<br>
model.add() 안에는 Dense() 함수가 포함되어 있다. -> 각 층이 각각 어떤 특성을 가질지 옵션을 설정하는 역할.<br>
딥러닝의 구조와 층별 옵션을 정하고 나면 compile()함수를 이용해 이를 실행시킴.<br>
* loss, optimizer, activation<br>
블랙박스를 극복하려면?

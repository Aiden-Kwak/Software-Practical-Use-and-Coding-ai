# Software-Practical-Use-and-Coding-ai
deep learning part

#1
Sequential 함수는 딥러닝의 구조를 한층 한층 쉽게 쌓아올릴 수 있게함. Sequential 함수 선언 후 케라스의 model.add() 함수 사용해 필요한 층을 차례로 추가하면 됨.<br> 
케라스의 장점 중 하나는 model.add() 함수를 이용해 필요한 만큼의 층을 빠르고 쉽게 쌓을 수 있다는 것.<br>
model.add() 안에는 Dense() 함수가 포함되어 있다. -> 각 층이 각각 어떤 특성을 가질지 옵션을 설정하는 역할.<br>
딥러닝의 구조와 층별 옵션을 정하고 나면 compile()함수를 이용해 이를 실행시킴.<br>
* loss, optimizer, activation<br>
블랙박스를 극복하려면?

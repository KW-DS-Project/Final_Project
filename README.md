# Final_Project
2019 자료구조실습 팀 프로젝트 결과물


g++ -o main.out menuClass.cpp people.cpp main.cpp order.cpp

main.out 만드는 법

*******************************************************************************

g++ -o client.out client.cpp

client.out 만드는 법

*******************************************************************************


MsgList구조체는 메뉴하나, 메뉴당 수량 정보 가지고 있다.

MsgCus는 주문 번호 (num ) , MsgList구조체의 배열, MsgList구조체의 배열이 30개인데 그게 다 메뉴이지는 않으므로, 쓸모있는 정보만 추출
편하도록 하는 menuTotal이있다

menuTotal 까지 for문을 돌리면 쓸모있는 메뉴가 다 등장한다.
만약, 0개인 메뉴를 제외하고 싶으면 내가 client.out 처럼 구현한대로 menuTotal 까지 for문돌린 후, if문으로 0개인 정보 제외하고 출력하면 된다.


********************************************************************************

메뉴를 바꾸고 싶다고 하면

g++ -o inputMenu.out inputMenu.cpp menuClass.cpp

./inputMenu.out 으로 실행 후 바꿈

*********************************************************************************

실행 순서 

g++ -o inputMenu.out inputMenu.cpp menuClass.cpp

g++ -o main.out menuClass.cpp people.cpp main.cpp order.cpp
g++ -o client.out client.cpp -lpthread
g++ mainServ.cpp -o mainServer.out -lpthread
g++ server2.cpp -o server.out -lpthread

./main.out
./client.out
./mainServer.out
./server2.out

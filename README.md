# [목차]
1.[게임명: 너구리fly](#게임명--너구리fly)  
2.[컨셉](#컨셉)  

# [게임명: 너구리fly]
지구를 지키기 위해 너구리들이 날기 시작하여 적과 싸움


# 컨셉
종스크롤 비행 슈팅게임  
서브컨셉1 플레이어는 2가지 캐릭터를 고를 수 있음  
서브컨셉2 스테이지를 추가해 클리어 할 수록 난이도가 높아짐  
서브컨셉3 플레이어는 미세한 컨트롤 능력이 요구됨

# 관련이미지
<img src="/imgs/image1.jpg" widht="300" height="300">  
<img src="/imgs/image2.jpg" widht="300" height="300">  

# 대표 이미지
<img src="/imgs/gameimage.png" widht="500" height="700">  

# 구성 요소
종스크롤 비행 슈팅게임
## 1. 메커니즘
[도전과제]  
당신은 너구리 힘을 이용해 마지막 최종보스까지 잡아라!  
[재미요소]
컨트롤을 요구하면서 강해진다.

## 2. 이야기
너구리들이 적의 침략에 맞서 지구를 지키기 위해 알 수 없는 힘을 얻게 되어 날기 시작했다.    
그 알 수 없는 힘을 얻으려면 바로 플레이어가 조종을 해야 얻을 수 있다.  

## 3. 미적 요소
[디자인]  
2D도트 그래픽으로 이질감없이 누구나 할 수 있는 느낌을 줄 수 있음  

[컬러]  
딱딱한 색이 아닌 부드러운 색을 이용함  

[음향]  
게임 배경음으로 심심하지 않게 게임을 이용할 수 있음  
플레이어와 적 들이 공격과 피격시에 효과음을 넣음  

## 4. 기술  
유니티2D 사용

# 게임 시스템 디자인  
1. 게임 오브젝트 분해  

|번호|오브젝트 이름|오브젝트 이미지|
|:---:|:---:|:---:|
|1|Player|<img src="/imgs/player.png" widht="200" height="200">|  
|2|enemy|<img src="/imgs/enemy.png" widht="200" height="200">|
|3|enemyboss|<img src="/imgs/boss.png" widht="200" height="200">|
|4|bullet|<img src="/imgs/bullet.png" widht="100" height="100">|  
|5|boom|<img src="/imgs/Boom_Game.png" widht="200" height="200">|
|6|item|<img src="/imgs/Item_Coin.png" widht="100" height="50"> <img src="/imgs/Item_Power.png" widht="100" height="50"> <img src="/imgs/Item_Boom.png" widht="100" height="50">|
|7|BackGround|<img src="/imgs/backgroundA.png" widht="100" height="150"> <img src="/imgs/backgroundB.png" widht="100" height="150"> <img src="/imgs/backgroundC.png" widht="100" height="150">|

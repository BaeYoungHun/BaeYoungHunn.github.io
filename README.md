# [게임 파일 다운로드](https://drive.google.com/file/d/13IZpBaZXxnmJeDXGQqm45Vh5V59gnOYZ/view?usp=sharing)
# [목차]
1.[게임명: 너구리fly](#게임명--너구리fly)  
2.[컨셉](#컨셉)  
3.[관련이미지](#관련이미지)  
4.[대표이미지](#대표이미지)  
5.[구성요소](#구성요소)  
6.[게임 시스템 디자인](#게임-시스템-디자인)  
7.[개발 요구사항 & 흐름도](#개발-요구사항--흐름도)  
8-1.[1주차 작업 결과](#1주차-작업-결과)  
8-2.[2주차 작업 결과](#2주차-작업-결과)  
8-3.[3주차 작업 결과](#3주차-작업-결과)  
8-4.[4주차 작업 결과](#4주차-작업-결과)  
8-5.[5주차 작업 결과](#5주차-작업-결과)  
8-6.[6주차 작업 결과](#6주차-작업-결과)  
8-7.[7주차 중간고사 발표](#7주차-중간고사-발표)  
8-8.[8주차 작업 결과](#8주차-작업-결과)  
8-9.[9주차 작업 결과](#9주차-작업-결과)  
8-10.[10주차 작업 결과](#10주차-작업-결과)  
8-11.[11주차 작업 결과](#11주차-작업-결과)  
8-12.[12주차 작업 결과](#12주차-작업-결과)  
8-13.[13주차 작업 결과](#13주차-작업-결과)  
8-14.[14주차 작업 결과](#14주차-작업-결과)  
8-15.[15주차 중간고사 발표](#15주차-기말고사-발표)  

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

# 대표이미지
<img src="/imgs/gameimage.png" widht="500" height="700">  

# 구성요소
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
## 1. 게임 오브젝트 분해  

|번호|오브젝트 이름|오브젝트 이미지|
|:---:|:---:|:---:|  
|1|Player|<img src="/imgs/player.png" widht="200" height="200">|  
|2|enemy|<img src="/imgs/enemy.png" widht="200" height="200"> <img src="/imgs/BEnemy2.png" widht="200" height="200">|  
|3|enemyboss|<img src="/imgs/boss.png" widht="200" height="200">  <img src="/imgs/boss2.png" widht="200" height="200">|  
|4|bullet|<img src="/imgs/bullet.png" widht="100" height="100">  <img src="/imgs/Enemybulletgohst.png" widht="100" height="100">|  
|5|boom|<img src="/imgs/Boom_Game.png" widht="200" height="200">|  
|6|item|<img src="/imgs/Item_Coin.png" widht="100" height="50"> <img src="/imgs/Item_Power.png" widht="100" height="50"> <img src="/imgs/Item_Boom.png" widht="100" height="50"> <img src="/imgs/item_life.png" widht="100" height="50"> <img src="/imgs/item_speed.png" widht="100" height="50">|  
|7|BackGround|<img src="/imgs/backgroundA.png" widht="200" height="250"> <img src="/imgs/backgroundB.png" widht="200" height="250"> <img src="/imgs/backgroundC.png" widht="200" height="250">  <img src="/imgs/backgroundA2.png" widht="200" height="250"> <img src="/imgs/backgroundB2.png" widht="200" height="250">|   
|8|Follower|<img src="/imgs/Follower.png" widht="50" height="50">|    

## 2. 파라미터(속성) 뽑아 보기
### 1)오브젝트 이름: Player

|속성|입력 값|설명|
|:---:|:---:|:---:|
|생명|3|플레이어 목숨|
|점수|0|플레이어의 점수|
|파워등급|1~6|플레이어의 파워 등급|
|총알속도|0.3|플레이어의 공격|
|스피드|2|플레이어의 이동속도|
|폭탄|0|플레이어의 폭탄|

### 2)오브젝트 이름: Enemy

|속성|입력 값|설명|
|:---:|:---:|:---:|
|Enemy|L, M, S, B|이름에 따라 생성되는 스프라이트|
|Enemy Health|200, 40, 5, 3500|적의 체력|
|Enemy score|500, 100, 50, 5000|적을 죽이면 얻는 점수|
|Enemy Speed|1, 6, 3, 1.5|적의 이동속도|
|Enemy2 Speed|3, 10, 5, 1.5|적의 이동속도|
|Enemy Bullet|A, B, C, D|적의 총알 구분|

### 3)오브젝트 이름: Bullet

|속성|입력 값|설명|
|:---:|:---:|:---:|
|BulletA|3|총알 이름-공격|
|BulletB|7|총알 이름-공격|
|FollowerBullet|3|총알 이름-공격|

### 5)오브젝트 이름: Item

|속성|입력 값|설명|
|:---:|:---:|:---:|
|item_Coin|score +1000| 먹으면 스코어 점수 1000 올라감|
|item_Power|Power++, maxPower일시 score +300|먹으면 파워 등급이 올라감 맥스파워일때 먹을경우 스코어점수 300이 올라감|
|item_Boom|Boomr++, maxBoom일시 score +300|먹으면 폭탄 갯수가 올라감 맥스폭탄일때 먹을경우 스코어점수 300이 올라감|
|item_Life|Life++, maxLife일시 score +300|먹으면 라이프 갯수가 올라감 맥스라이프일때 먹을경우 스코어점수 300이 올라감|
|item_Speed|이동속도 0.5 공격속도 0.02씩 오름 maxSpeed일시 score +300|먹으면 이동속도와 공격속도가 오름 맥스스피드일때 먹을경우 스코어점수 300이 올라감|

### 4)오브젝트 이름: Item_Boom

|속성|입력 값|설명|
|:---:|:---:|:---:|
|enemy destory|ture|적 제거|
|enemy bullet destory|true|모든 적 총알 제거|

## 3. 행동 뽑아 보기
### 1)오브젝트 이름: Player

|행동|설명|
|:---:|:---:|
|이동|W A S D or 방향키로 플레이어이동|
|총알 발사|"스페이스바"키로 총알 발사|
|폭탄|"K"키로 총알 발사|

### 2)오브젝트 이름: Enemy

|행동|설명|
|:---:|:---:|
|이동|좌-우 이동, 상(上)에서 하(下)로 이동|
|총알 발사|플레이어를 향해서 총알 발사|

### 3)오브젝트 이름: Item

|행동|설명|
|:---:|:---:|
|생성|적을 잡으면 확률적으로 코인 또는 아이템이 생성됨|
|충돌|아이템과 충돌시 사라지고 플레이어에게 효과가 생김|
|플레이어 강화|충돌한 오브젝트에 따라 폭탄, 생명이 생기거나 파워,공이속 업그레이드 됨|

## 4.상태 뽑아 보기
### 1). 오브젝트 이름: Player

|현 상태|전이상태|전이조건|
|:---:|:---:|:---:|
|정상|상으로 이동 상태|상 방향키 눌림|
|정상|하으로 이동 상태|하 방향키 눌림|
|정상|좌로 이동 상태|왼쪽 방향키 눌림|
|정상|우로 이동 상태|오른쪽 방향키 눌림|
|정상|공격|공격키 눌림|

### 1). 오브젝트 이름: Enemy

|현 상태|전이상태|전이조건|
|:---:|:---:|:---:|
|스폰|이동|적 스폰후 이동|
|이동|제거|소환되고 맵밖으로 사라질시에 제거|
|이동|사망|플레이어에게 공격을 맞고 체력이 0이 되었을 때 확률적으로 아이템 생성|


## 4.게임의 규칙
### 1)핵심 규칙  
플레이어는 적을 제거하고 보스를 잡아라  
### 2)보조 규칙
플레이어는 생명이3개, 폭탄을 가질 수 있다.  

# 개발 요구사항 & 흐름도 
## 1.요구사항(중간고사전 / 기말고사전)]
### 중간고사전 요구사항
-플레이어 생성  
-플레이어 목숨 생성  
-플레이어 애니메이션 생성  
-플레이어 총알 생성  
-적 생성과 피격이벤트 생성  
-적 플레이어 공격  
-아이템 생성  
-플레이어와 아이템 충돌시 먹을 수 있음  
-사운드 효과 생성  
-패럴랙스 효과로 원근감있게 생성  
-점수 생성  
-보스 생성  
-보스 패턴 생성  
-팔로워 생성  
-팔로워 총알은 관통  
### 기말고사전 요구사항
- 다른분위기 스테이지
- 다른스테이지 보스추가, 몬스터 추가
- 몬스터가 물결파형으로 움직이게 추가
- 몬스터가 플레이어쪽이동 추가
- 다른스테이지 몬스터가 살짝투명해졌다가 선명해졌다가 반복해 보임
- 보스 좌우로 이동
- 보스 2개 패턴 추가
- 인트로 그림 화면 추가
- 라이프 아이템 추가
- 공이속 아이템 추가

## [1주차 작업 결과]  
구상 및 계획  

## [2주차 작업 결과]  
플레이어 이동   
플레이어 이동시 애니메이션효과  
패럴랙스 배경생성  
<video width="100%" height="100%" controls="controls">
  <source src="/video/1wnck.mp4" type="video/mp4">
</video>

## [3주차 작업 결과]
적 생성  
적 피격시 이벤트 발동
적 스폰지역 설정  
플레이어 공격 생성  
<video width="100%" height="100%" controls="controls">
  <source src="/video/2wnck.mp4" type="video/mp4">
</video>

## [4주차 작업 결과]
UI생성
점수 생성
아이템 생성(코인, 파워업, 폭탄)  
"K" 키를 누르면 폭탄이 
적이 플레이어 방향으로 공격을 함  
적 또는 플레이어가 죽으면 파티클 효과 생성  

<video width="100%" height="100%" controls="controls">
  <source src="/video/3wnck.mp4" type="video/mp4">
</video>

## [5주차 작업 결과]
스테이지 관리 생성  
보스 생성  
보스패턴 생성  
여러가지 효과음 생성  

<video width="100%" height="100%" controls="controls">
  <source src="/video/4wnck.mp4" type="video/mp4">
</video>  

## [6주차 작업 결과]  
팔로워 생성  
팔로워 총알은 적을 관통함  
죽은 후 일정시간동안 무적  

<video width="100%" height="100%" controls="controls">
  <source src="/video/5wnck.mp4" type="video/mp4">
</video>

## [7주차 중간고사 발표]  
----  

## [8주차 작업 결과]  
게임 스타트 UI  

<img src="/imgs/8wnck.png" widht="300" height="650">

## [9주차 작업 결과]  
게임 스테이지 추가(같은 맵으로 추가했음)  

## [10주차 작업 결과]  
씬 Intro 추가와 스테이지2추가, END추가 그리고  
스테이지2 다른분위기로 추가 했지만 실패물  

<img src="/imgs/intro.png" widht="300" height="650"><img src="/imgs/End.png" widht="300" height="650"><img src="/imgs/stage2.png" widht="300" height="650">

## [11주차 작업 결과]  
교수님 피드백으로 스테이지를 완전히 바꿈  
그리고 맵 컨셉에 맞게 몹들이 투명해졌다가 다시 돌아왔다가 반복함  
<img src="/imgs/11wnck.png" widht="300" height="650"><img src="/imgs/11_2wnck.png" widht="200" height="150">

## [12주차 작업 결과]  
몬스터가 물결로 내려옴  
몬스터가 플레이어 위치로 내려옴  
보스 몬스터 추가  

![11wnck](https://user-images.githubusercontent.com/101154099/174482128-7cbf578e-733f-423b-90f2-8939dc584f73.gif)  

<img src="/imgs/12wnck.png" widht="300" height="300">

## [13주차 작업 결과]  
intro화면 그림화면 추가...  
보스가 좌우로 움직임  
<img src="/imgs/intro22.png" widht="300" height="300">  
![13wnck](https://user-images.githubusercontent.com/101154099/174483128-99b4446e-1d29-4db3-89d9-0f9a0e1b584a.gif)

## [14주차 작업 결과]  
아이템 2개 추가  
보스패턴2개 추가   
![14_1wnck ](https://user-images.githubusercontent.com/101154099/174484590-fabfaf27-0af5-4711-94cb-03cdb54d17ce.gif)  
![14_2wnck ](https://user-images.githubusercontent.com/101154099/174484604-438372c2-31e2-43be-bae0-8e691fa88261.gif)  
![14_3wnck](https://user-images.githubusercontent.com/101154099/174484643-724e2cae-e7c4-48af-b31c-f2a081e6352a.gif)  

## [15주차 기말고사 발표]  
-----------  

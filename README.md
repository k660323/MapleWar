# [Maple World] Maple War
## 1. 소개

<div align="center">
  
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%EB%A9%94%EC%9D%B8%20%ED%99%94%EB%A9%B4.PNG" width="49%" height="400"/>
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%EB%84%A4%EC%9E%84%ED%83%9C%EA%B7%B8%20%EC%8A%A4%ED%82%A8%20%ED%8C%90%EB%A7%A4.PNG" width="49%" height="400"/>
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%ED%94%BC%EA%B2%A9%20%EC%8A%A4%ED%82%A8%20%ED%8C%90%EB%A7%A4%20%EC%B2%AD%EC%9D%B4.PNG" width="49%" height="400"/>
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%EC%9D%B8%EB%B2%A4%ED%86%A0%EB%A6%AC.PNG" width="49%" height="400"/>
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%EB%A7%A4%EC%B9%AD%20%EC%A4%80%EB%B9%84.png" width="49%" height="400"/>
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%EC%A7%84%EC%98%81%20%EC%84%A0%ED%83%9D.JPG" width="49%" height="400"/>
  <img src="https://github.com/k660323/MapleWar/blob/main/Images/%EC%A0%84%ED%88%AC%20%EC%95%95%EC%B6%95%ED%8E%B8.png" width="99%" height="600"/>
  
  < 게임 플레이 사진 >
</div>

+ Malple War란?
  + 1:1 ~ 3:3 까지 AI 및 플레이어와 대전이 가능한 실시간 전략 시뮬레이션 게임입니다.
 
+ 목표
  + 소환수를 소환하여 상대팀 기지를 파괴하면 이기는 게임입니다. (전쟁 시대 게임과 유사)

+ 게임 흐름
  + 게임 시작시 정해진 시간안에 숫자가 적힌 카드를 선택해주시면 됩니다. (주사위를 굴릴 순서)
  + 그 후 내차례에 주사위를 굴러 나온숫자만큼 움직입니다.
  + 해당 땅에 도착했을시
  + 일반 지역이면 땅을 살 수 있다. 만약 상대팀 땅이면 통행료를 지불하고 땅을 매입할 수 있다. 만약 통행료가 없으면 파산처리가 된다. 특수 지역이면 설정된 이벤트 발생
  + 이 흐름이 반복되어 라인 독점, 관광지 독점, 또는 상대팀 파산을 시켜 이길 수 있다.        

+ 게임 규칙
  + 매 턴 마다 소환수를 소환하고 턴이 지나면 다음 턴이 올때까지는 소환수를 소환 하실수 없습니다.


<br>

## 2. 프로젝트 정보

+ 사용 엔진 : Maple World
  
+ 엔진 버전 : Project MOD (클로즈 베타 테스트)

+ 사용 언어 : Lua
  
+ 작업 인원 : 1명
  
+ 작업 영역 : 콘텐츠 제작, 디자인, 기획
  
+ 장르      : 전략 시뮬레이션
  
+ 소개      : 넥슨 자체 엔진인 Maple World를 활용하여 만든 멀티플레이 전략 시뮬레이션 게임
  
+ 플랫폼    : PC / Mobile
  
+ 개발기간  : 2021.11.17 ~ 2022.02.09
  
+ 형상관리  : GitHub Desktop

<br>

## 3. 게임 설명

**상단 패널**
| 명칭 | 설명 |
|:---:|:---|
| 시간 증폭  | 10초간 생산력을 2배 증가합니다. |
| 포탑  | 지속시간이 있는 포탑을 생성하실수 있습니다. |
| 미르  | 기지 앞에 있는 소환수를 멀리 날려 버립니다. |
| 소환수 저장 | 소환수를 Queue에 저장합니다. |
| 기지 복귀 |  카메라를 자신의 기지로 이동시킵니다. |
| 시그니처(궁극의 소환수) | 강력한 소환수를 소환합니다. 강력한 스킬을 사용 가능합니다. |

**하단 패널**
| 명칭 | 설명 |
|:---:|:---|
| 메소 업 | 초당 얻을 수 있는 메소량을 상승시킬수 있습니다. |
| 티어 업 | 더 강한 소환수를 소환할 수 있습니다. |
| 소환수 | Q : 근접형, W : 원거리, E : 버프/디버프,  R ,T 근거리 또는 원거리 특화된 소환수 |
| 소환수 저장 | 소환수를 Queue에 저장합니다. |
| 기지 복귀 |  카메라를 자신의 기지로 이동시킵니다. |
| 폭탄 | 기지 앞에 있는 모든 소환수를 제거합니다. |

<br>

<br>

---

<br>

## 4. 구현에 어려웠던 점과 해결과정
+ MOD란 게임 엔진을 처음 써보았고 첫 베타 테스트이기 때문에 미 구현된 기능(애니메이션 이벤트), 그리고 MOD에서 지원하는 함수 작동 로직에 대해 잘 몰랐고, 처음 써보는 Lua 언어였기 때문에 개발에 많은 어려움이 있었습니다.
  + 오류나 필요 기능이 누락 되었을 경우 Discord로 문의함으로써 추후에 패치 되도록 건의하였습니다. 

 
## 5. 느낀점
+ 새로운 Lua Script 언어를 접했다.
+ 코드의 설계가 얼마나 중요한지 깨달았다. 공모전을 하면서 만든 코드들이 점점 많아질 때 마다 점점 코드들을 추가하고 이해하기 어려웠다. 상속과 클래스들을 의미를 두고 코딩을 해야함을 깨달았다.
+ 데이터 시트를 만들어 손쉽게 데이터를 정의하고 데이터를 접근 할 수 있다.
+ 공모전을 하면서 나보다 아이디어가 좋고 연출이 좋은 분들이 많다고 느꼈다. 

## 6. 플레이 영상
+ https://www.youtube.com/watch?v=IdTsry-v_B8

## 7. 게임 링크
+ https://maplestoryworlds.nexon.com/ko/play/198d931285cc4fa49556fd5ffa91785a/

## 8. PDF
+ https://github.com/k660323/MapleWar/blob/main/PDF/Maple%20War.pdf

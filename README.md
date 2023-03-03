# FiFa4_API_project

## 프로젝트 주제 
> FiFa 온라인 4의 게임 데이터 중 상위 랭커들의 선수 활용기록과 그 선수의 능력치 간의 관계를 회귀분석하여 포지션별 필요한 선수를 잘 선택하도록 하자!
> - 예) 'CF의 포지션의 선수 중 유효슈팅을 잘 때리는 선수를 고르고 싶은데 어떤 능력치가 높아야될까?'와 같은 질문을 해결하기  

## 프로젝트 목적
> 1. 전에 공부한 정적 크롤 방법과 제공된 API키를 이용해 데이터 수집하기
> 2. 수집한 데이터를 전처리과정을 통해 가공하기
> 3. 회귀 분석을 하기

## 프로젝트 설명
### 설계 
> 1. 넥슨에서 제공된 게임 API를 이용하여 선수들의 ID와 랭커들의 선수 활용 기록을 구한다. 
> 2. 선수 ID를 이용해 fifa4 데이터센터에서 맞는 선수의 능력치를 크롤링 한다.
  - 이 때 선수는 약 3만명으로 많아 fafa4 데이터센터에서 능력치 순 포지션별 탑 5명씩 선택해 진행하였다. 
> 3. 구한 랭커들의 활용 기록과 능력치끼리의 회귀 분석을 통해 활용 목적에 따른 필요 능력치를 구한다.
 
### main 파일
> 데이터를 작은 요소부터 수집을 하고 필요한 부분을 가공하기 위한 실습 파일

### fanal_code 파일
> 실습 파일로 얻은 코드들을 정리한 최종 프로젝트 파일
#### 
  1. all_players_spId_position
    > API url를 활용하기 위해 선수 spId와 포지션 묶어주는 함수
  2. def rankers_used_func
    > API를 이용해 선수와 포지션별 랭커 선수 활용 데이터를 구하는 함수
    
  

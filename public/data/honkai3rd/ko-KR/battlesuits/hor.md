# 이치의 율자

## 누메론 프로토콜

리더로 배치 시 파티원이 버프를 받는다.
누메론 프로토콜: 전체 파티원의 모든 원소 대미지가 30.0% 증가하고 파티 내 브로냐, 제레, 아린 자매의 모든 대미지가 25.0% 증가한다.

### 구현 해석

라이드 모드가 아닐 때 차지 공격은 원소 관통력을 10.0% 획득한다.

### 누메론 프로토콜

전체 파티원의 모든 원소 대미지가 30.0% 증가하고 파티 내 브로냐, 제레, 아린 자매의 모든 대미지가 25.0% 증가한다.

### 천리 재구성

라이드 모드 상태에서 퇴장 시 캐릭터는 구조 에너지를 240pt, SP를 10.0pt 회복한다.

## 패시브 스킬

패시브 스킬은 자동으로 발동된다.
구조 에너지: 최대치 480pt
적에게 해석 상태를 부여할 때 적은 1.5초 동안 빙결 상태가 되고 해당 적에게 가하는 모든 대미지가 40% 증가한다.
퇴장 시 율자 모드에서 벗어나고 중장 토끼는 인간 형태로 돌아온다

### 2패스 코딩

기본 구조 에너지 360pt 증가.

### 빌드 리부트

스테이지 위의 중장 토끼가 모터사이클에서 인간 형태로 돌아올 때 캐릭터가 스테이지에 있으면 구조 에너지를 240pt 회복한다.

### 모드 전환

차지 공격으로 가하는 빙결 원소 대미지 72% 증가.

## 급속 제동

빠르게 적의 공격을 회피하며 연속으로 2회 회피할 수 있다.
극한 회피 시 자신의 구조 에너지를 120pt 회복하고 1.7초 내에 다음 공격을 발동하면 적을 4초 동안 해석 상태로 만든다.
급속 제동: 극한 회피 시 3초 동안 시공 단열을 발동한다. 재사용 대기시간: 15초

### 프리즈 트레쉬홀드

급속 제동의 재사용 대기시간이 3.0초 감소하고 급속 제동의 시공단열에 영향받은 적은 6초간 해석 상태에 진입한다.

### 비상 댐퍼

급속 제동 발동시 추가로 HP를 400pt 회복한다. 급속 제동이 재사용 대기 중이 아닐 때 피격 후 짧은 시간 안에 회피를 사용해 급속 제동을 발동할 수 있다.

### QTE - 데이터 스톰

QTE: 적이 마비 혹은 시공 단열일 때 발동하여 적에게 공격력의 500.0%의 물리 대미지+공격력 500.0%+300%의 빙결 원소 대미지를 입히고 구조 에너지를 120pt 회복한다. 적중한 적에게 6초간 해석 상태를 부여한다.

## 차지 - 무기화 빌드

4연격과 회피 시 차지하여 차지 공격을 발동한다.
차지 공격은 120pt의 구조 에너지를 소모하여 율자 형태로 진입한다. 이 기간 동안 공격 버튼을 누르면 차지 동작이 끝나기 전까지 바로 차지 공격을 발동할 수 있다.
무기 구조: 무기 유형에 따라 다른 차지 공격방식을 사용할 수 있으며 총 공격력 660%의 빙결 원소 대미지를 입힌다.

### 데이터 질주

율자 형태: 적에게 가하는 모든 대미지가 30.0% 증가 하고 이능 속성의 적에게 가하는 모든 데미지가 추가로 40% 증가한다.

### 방화벽

율자 형태: 받는 모든 데미지가 50% 감소한다.

### 스트림 트랜스퍼

율자 형태: 라이드 모드가 아닐 때 차지 공격할 때마다 SP를 5.0pt 회복하고 빙결 원소 대미지가 15.0% 증가한다. 대미지 증가 최대 중첩 횟수: 3회

## 사이버 엔젤.cfg

중장 토끼가 변신하여 폭발 상태에 진입한다.
구조 에너지를 480pt 회복하고 적에게 공격력 5\*450%+800%의 빙결 원소 대미지를 입히고 라이드 모드에 진입하고 율자 형태가 된다. 최대 지속시간: 17초
라이드 모드: 이 기간 동안 캐릭터는 전투 불능이 되지 않고 초당 40pt의 구조 에너지를 회복한다. 이동 시 0.6초마다 호버 레이저포를 구조하여 적에게 공격력 4\*65%의 빙결 원소 대미지를 입힌다.
공격 버튼: 구조 에너지 240pt 소모, 바로 차지 공격 발동 시 적에게 공격력 2\*250%+2\*300%의 빙결 원소 대미지를 입히고 4초 동안 해석 상태를 부여한다.
회피 버튼: 회피하는 동안 적중한 적에게 최대로 공격력 4\*10%의 빙결 원소 대미지를 입히고 4초 동안 해석 상태를 부여한다.
재사용 대기시간: 30초, 발동 시 SP 소모: 125

### 빠른 디크립션

라이드 모드: 차지 공격 시 20.0%의 모든 원소관통을 획득한다.

### 언더클럭

라이드 모드: 받는 간접 피해량 30.0% 감소

### Rebuild.exe

라이드 모드: HP가 50% 미만일 때 0.5초마다 40.0pt의 HP를 회복하고 HP가 25% 미만일 때 0.5초마다 추가로 60.0pt의 HP를 회복한다.

## 제로 드라이브

4연격
제1격: 공격력 100%의 물리 대미지 + 공격력 80%의 빙결 대미지
제2격: 공격력 100%의 물리 대미지+ 공격력 100%의 빙결 원소 대미지,
구조 에너지 25pt 회복
제3격: 공격력 150%+150%의 물리 대미지 + 공격력 2\*100%의 빙결 원소 대미지,
구조 에너지 25pt 회복
제4격: 드릴을 만들어내 공격력 8\*40%+200%의 빙결 원소 대미지를 입히고
9\*25pt의 구조 에너지를 회복하며 작은 범위의 적을 끌어당긴다.

### 구조 분석

드릴 공격이 끝난 후의 임팩트는 피격된 적에게 6.00초 동안 해석 상태를 부여한다.

### 파워 링크

드릴 공격이 적을 명중할 때마다 SP를 0.50pt 회복한다.

### 스톱 어레이

드릴 공격 중 정면과 측면은 공격에 면역되고 후방에서 받는 모든 대미지가 30% 감소한다.

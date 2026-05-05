# CN Tracker DNS Filter

[🇺🇸English/영어](./README.md)

## 개요

CN Tracker DNS Filter는 Alibaba, Tencent, Baidu, ByteDance와 같은 주요 플랫폼에서 사용하는 중국계 추적, 광고, 텔레메트리 도메인을 대상으로 하는 DNS 레벨 차단 필터이다.

이 필터는 일반적인 광고 차단 필터를 대체하는 것이 아니라, 보완용 필터로 설계되었다.


## 목적

이 필터의 목적은 다음과 같다:

- 중국계 광고 및 추적 인프라 차단
- 앱에 내장된 SDK의 텔레메트리 수집 감소
- 리디렉션 기반 추적 완화
- 기본 DNS 필터 이상의 개인정보 보호 강화


## 적용 범위

### 포함

- Alibaba 계열 (예: "mmstat", "tanx", "alimama")
- Tencent 계열 (예: "gdt", "beacon", "qq analytics")
- Baidu 분석 및 광고 시스템
- ByteDance 추적 엔드포인트
- 중국 모바일 SDK 트래커 (예: Umeng, TalkingData)

### 제외

- 글로벌 광고 네트워크 (기본 필터에서 처리)
- Cosmetic 필터링 (DNS 레벨에서는 적용 불가)
- 일반 웹사이트별 규칙


## 사용법

AdGuard / DNS 필터에 추가
#### [이 링크를 복사](https://github.com/mchany/CN-Tracker-DNS-Filter/blob/7c4380ae896ae56f47a0afd8ec7050cc7d2b32b8/CN%20Tracker%20DNS%20Filter.txt)


## 문제점

다음 도메인을 차단할 경우 일부 기능에 문제가 발생할 수 있음:

- "qq.com" / "tencent.com" → 로그인 또는 콘텐츠 문제
- "bdstatic.com" → 일부 리소스 누락
- 리디렉션 도메인 → 링크가 정상적으로 열리지 않을 수 있음

사용 환경에 따라 특정 도메인을 허용 목록에 추가해야 할 수 있음.


## 면책 조항

이 필터는 특정 지역의 추적 인프라를 대상으로 함.
일부 서비스의 기능에 영향을 줄 수 있음.

필요한 경우 사용자 정의 허용 규칙을 추가하여 조정이 필요할 수 있음.

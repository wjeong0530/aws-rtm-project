# 주제: AWS CloudWatch를 이용한 고가용성 모니터링 및 실시간 장애 대응 서비스
> [!NOTE]
> **프로젝트 기간:** 2026.05.11-2026.06.12 / **난이도:** ★★★★☆

## 주제로 선정한 이유
- 이유1
- 이유2
- 이유3

## 최신 동향과 발전 과제
- 이유1
- 이유2

## 프로젝트 구성도
![예시도면](./예시도면.png)

## 프로젝트 목표:
1. CloudFormation 템플릿을 사용한 AWS 기본 인프라 구축
2. OpenVPN Access Server를 활용한 안전한 원격 접속 환경 구축
3. ALB와 서브넷별 Openvpn 인스턴스를 통한 고가용성 확보
4. Auto Scaling Group을 통한 탄력적 운영 구현
5. ACM과 WAF를 활용한 웹서비스 보안 강화
6. EC2 + Apache + PHP 프론트엔드 구현
7. RDS를 활용한 회원가입 및 로그인 플랫폼 구축

## 프로젝트 일정계획
| 일차 | 날짜 | 내용 |
| --- | --- | --- |
| 1일차 |  | AWS 클라우드 프로젝트를 위한 사례 연구<br>프로젝트 주제 및 목표 설정<br>프로젝트 구성도 생성 |
| 2일차 |  | CloudFormation 템플릿을 사용한 AWS 기본 인프라 구축<br>OpenVPN Access Server를 활용한 안전한 원격 접속 환경 구축<br>ALB와 서브넷별 Openvpn 인스턴스를 통한 고가용성 확보<br>Auto Scaling Group을 통한 탄력적 운영 구현<br>ACM과 WAF를 활용한 웹서비스 보안 강화|
| 3일차 |  | EC2 + Apache + PHP 프론트엔드 구현<br>CloudWatch를 활용한 서버 모니터링 시각화 플랫폼 구축<br>결과 테스트 |
| 4일차 |  | 프로젝트 결과 정리<br>PPT 제작 |
| 5일차 |  | 프로젝트 결과 정리<br>PPT 제작 |

## 세부 내용:
1. 리전의 웹 서버는 ALB를 이용해 고가용성을 구성
2. 리전의 웹 서버는 Auto Scaling Group을 이용해 탄력적으로 확장되도록 구성
3. 서울 리전은 NAT Gateway를 사용
4. 서울 리전에 OpenVPN 인스턴스 2대를 설치하여 프라이빗 망을 구성
5. OpenVPN 및 전체 웹 서버는 각 리전의 키 페어(seoul-key)로 SSH 접속이 가능하도록 구성
6. 웹 클라이언트는 Route 53 DNS를 통해 웹 서버에 접속하도록 구성
---
Copyright (C) 2026. WJEONG

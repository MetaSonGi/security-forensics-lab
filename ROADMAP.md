# 보안 + 디지털 포렌식 통합 로드맵 (12주)

원칙: 모든 실습은 본인 소유 VM·랩·CTF·공개 샘플 데이터에서만 진행합니다.

## Phase 0. 공통 기초 & 랩 구축 (Week 1-2)
- VirtualBox/VMware: Kali Linux + Windows VM + Ubuntu Server, 스냅샷 습관화
- 네트워크: TCP/IP, DNS/HTTP, 포트/서비스 — Wireshark로 직접 캡처
- OS: Linux 권한/프로세스/저널, Windows 레지스트리/이벤트로그/NTFS
- 도구: Wireshark, Nmap, Python 3
- 완료 기준: VM 간 통신 확인 + HTTP 요청 1건 추적 가능

## Track A. 보안 (Week 3-6)
- A1 네트워크/시스템: Nmap은 본인 VM만, 열린 포트와 공격 표면, 서비스 축소 전후 비교
- A2 웹: OWASP Top 10, DVWA/Juice Shop 로컬 실습 — 재현 → 원인 → 패치 → 재검증
- A3 시스템: 권한상승 개념, 해시 원리(샘플 해시만), Metasploitable 랩 전용
- A4 탐지: 로그인 성공/실패 로그, Wazuh/Splunk 맛보기
- 산출물: 취약점 리포트 1편

## Track B. 디지털 포렌식 (Week 3-6)
- B1 원칙: 증거 보전, Chain of Custody, SHA-256 무결성, 이미징
- B2 디스크: 삭제 파일 원리, $MFT, 타임스탬프, Autopsy/PhotoRec
- B3 메모리/윈도우: Volatility 3, Prefetch, LNK, 이벤트로그
- B4 네트워크: pcap 세션 재구성, 디스크+메모리+네트워크 타임라인 통합
- 산출물: 증거 기반 케이스 리포트 1편 (사실과 추측 분리)

## Phase C. 통합 — OT/ICS 보안 + 사고대응 (Week 9-11)
- Modbus/TCP 구조, 네트워크 분리, Purdue 모델
- OT 트래픽 pcap 시나리오 분석 → 타임라인 복원 → 방어책
- 사고대응 플레이북: 탐지 → 격리 → 증거보전 → 복구

## 이후 확장
- CTF 주 1문제, 풀이 기록
- 자격증: 정보보안기사, 디지털포렌식전문가 등 검토

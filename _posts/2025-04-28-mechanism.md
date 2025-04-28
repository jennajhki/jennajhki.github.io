---
title: "Consensus Mechanism"
layout: single
tags: [blockchain, consensus, pow, pos, dpos, bft]
comments: true
---

Consensus Mechanism 블록체인 핵심 개념 쉽게 이해하기 🔗

Consensus Mechanism 합의 알고리즘이란 무엇인가?

탈중앙화된 네트워크의 여러 참가자들이 하나의 동일한 데이터 상태에 동의하고 기록하기 위해 사용하는 규칙과 절차

블록체인은 수많은 컴퓨터(노드)들이 "모두 같은 데이터를 가지고 있다"는 것을 믿을 수 있게 하는 시스템

합의 알고리즘의 역할

- 누가 새로운 블록을 추가할지 결정
- 네트워크에 부정확한 데이터(거짓 거래)를 막음
- 탈중앙화 상태에서도 신뢰trust 를 유지함

---

대표적인 합의 알고리즘 종류 4개

1. Proof of Work (PoW) - 작업증명
  * 예) 비트코인(BTC)
  * 컴퓨터로 어려운 수학문제 풀어야 블록만들 수 있음
  * 가장 먼저 문제를 푼 노드가 블록 추가 가능
  * 강력한 보안성
  * 에너지 소모 매우 큼

2. Proof of Stake (PoS) - 지분증명
  * 예시) 이더리움 2.0(ETH), Cardano(ADA)
  * 코인 staking해서 블록 생성 후보가 됨
  * 많은 지분을 가진 노드가 유리
  * 에너지 효율 높음
  * "코인을 많이 가진 부자"가 유리할 수 있음

3. Delegated Proof of Stake (DPoS) - 위임 지분 증명
  * 예시) EOS, Tron(TRX)
  * 코인 보유자가 대표자 Validator를 투표로 선출
  * 선출된 대표자가 블록 생성 및 검증
  * 속도 매우 빠름
  * 중앙화 위험 있음

4. Practical Byzantine Fault Tolerance (PBFT)
  * 예) Hyperledger Fabric, 일부 Private chain
  * 네트워크 참여자 다수가 서로 메시지를 주고받아 합의
  * 소수(1/3 미만)의 악성 노드가 있어도 시스템 작동
  * 빠른 합의 가능
  * 네트워크 부담이 큼 (메시지 교환량)

## 📊 Consensus Mechanism Comparison Table 합의 알고리즘 비교표

| Category | PoW | PoS | DPoS | PBFT |
|----------|-----|-----|------|------|
| **Block Creation Method** | Solve cryptographic puzzles | Stake coins to become eligible | Elected delegates create blocks | Consensus through message exchanges |
| **Speed** | Slow | Fast | Very fast | Very fast |
| **Energy Consumption** | Very high | Very low | Very low | Low |
| **Security Level** | Very high | High | Moderate | High |
| **Degree of Decentralization** | Very high | High | Can be low (due to delegate concentration) | Low (typically private chains) |
| **Representative Projects** | Bitcoin | Ethereum 2.0, Cardano | EOS, Tron | Hyperledger Fabric |


|------|-----|-----|------|------|
| Block Creation Method 블록 생성 방식 | 퍼즐 풀이 | 스테이킹 | 투표로 선출된 대표자 | 메시지 교환으로 합의 |
| Speed 속도 | 느림 | 빠름 | 매우 빠름 | 매우 빠름 |
| Energy Consumption 에너지 소비 | 매우 높음 | 매우 낮음 | 매우 낮음 | 낮음 |
| Security Level 보안성 | 매우 높음 | 높음 | 보통 | 높음 |
| Degree of Decentralization 탈중앙화 정도 | 매우 높음 | 높음 | 낮을 수 있음 | 낮음 (프라이빗) |
| Representative Projects 대표 사용 프로젝트 | 비트코인 | 이더리움 2.0 | EOS, Tron | Hyperledger |

---


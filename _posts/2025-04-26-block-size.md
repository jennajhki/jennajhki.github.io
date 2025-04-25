---
title: "Bitcoin Block Size: Why It’s Not Just 1MB or 4MB"
layout: single
tags: [bitcoin, blockchain, segwit, block-size]
comments: true
---

# 비트코인 블록 크기, 진짜 4MB일까?

많은 사람들이 "비트코인 블록 크기 = 4MB"라고 알고 있지만,  
사실 이건 정확히 말하면 **"block weight 기준 최대 4MB"**라는 의미입니다.

비트코인의 실제 블록 구조와 함께, 왜 이런 오해가 생겼는지 이해해봅시다.

---

## 원래 비트코인의 블록 크기 제한: **1MB**

비트코인은 초기에 **각 블록의 크기를 1MB로 제한**했어요.

- 목적: 네트워크 과부하 및 DDoS 공격 방지
- 사토시가 코드에 직접 넣은 제한
- 평균 트랜잭션 크기: 약 250~500 byte

이 구조 덕분에 비트코인은 초기엔 가볍고 안전했지만,  
이후 **트랜잭션 혼잡 → 수수료 급등** 문제가 발생했죠.

---

## 2017년, SegWit의 등장

**SegWit (Segregated Witness)** 업그레이드는  
비트코인의 **확장성 문제 해결**을 위해 2017년 도입되었습니다.

### 핵심 변화:

- 트랜잭션 내 서명(Signature) 데이터를 **블록 외부(witness 영역)**로 분리
- 새로운 개념: **Block Weight** 도입

---

## Block Weight 계산 방식

SegWit 이후, 블록의 크기를 다음과 같이 계산합니다

Block Weight = (stripped size × 3) + total size

---
layout: single
title: "Digital Signature"
---

Timestampe Authority TSA 타임스템프 인증 기관
* 데이터 무결성 증명
* 시간 인증
* 신뢰 제공

비트코인에서 디지털 서명
* transaction 무결성 보장: 서명 유효성
* 소유권 증명
* 탈중앙화된 검증

검증 과정
1. 서명 생성
2. transanction 데이터 준비
3. 해싱
4. 개인 키를 사용한 서명: 송신자가 자신의 개인키로 해시 값을 서명
   * ECDSA(Elliptic Curve Digital Signature Algorithm)사용해 디지털 서명 생성
5. 서명과 transanction 데이터 전송
6. transanction 데이터 해싱
7. 공개 키를 사용한 검증
8. 검증 결과: 서명이 유효하면 transanction을 네트워크에 추가함

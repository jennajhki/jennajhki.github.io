---
title: "How the Web Works: Understanding HTML, HTTP, URL, Client, and Server "
layout: single
tags: [web, html, http, url, server, client]
comments: true
---

# 웹의 기본 구성요소

HTML, HTTP, URL, 클라이언트(Client), 서버(Server)

## HTML (HyperText Markup Language)

- **HTML**은 웹페이지를 구성하는 뼈대다.
- 웹브라우저가 읽을 수 있는 언어로, 텍스트, 이미지, 링크 등을 정의한다.

---
<pre><code>
<h1>Hello, Web!</h1>
<p>이건 HTML로 만든 문단입니다.</p>
</code></pre>

---<pre><code>
<h1>Hello, Web!</h1>
<p>이건 HTML로 만든 문단입니다.</p>
</code></pre>----
---

## URL (Uniform Resource Locator)
URL은 웹상 자원의 "주소"

우리가 주소창에 입력하는 https://www.example.com/about 같은 것

---
예시) https://www.example.com:443/about?page=1

| 구성 요소    | 값                    | 설명 |
|-------------|-----------------------|------|
| **Protocol** | `https`               | 통신 방식 (보통 http 또는 https) |
| **Domain**   | `www.example.com`     | 서버 주소 (호스트 이름) |
| **Port**     | `443`                 | 통신에 사용하는 포트 번호 (생략 가능, https의 기본은 443) |
| **Path**     | `/about`              | 요청한 리소스의 경로 |
| **Query**    | `?page=1`             | 서버에 전달할 추가 정보 (쿼리 문자열) |

---

## HTTP (HyperText Transfer Protocol)

HTTP는 클라이언트와 서버가 데이터를 주고받기 위한 약속(프로토콜)

## Client (클라이언트)
웹브라우저(Chrome, Safari 등)처럼,
서버에 요청을 보내는 주체를 클라이언트라고 한다.

사용자의 기기에서 실행되고,

URL을 통해 서버에 요청을 보내고,

HTTP 응답을 받아서 HTML을 화면에 보여준다

## Server (서버)
요청을 받아서 응답을 돌려주는 컴퓨터(또는 프로그램)

클라이언트가 "이 주소의 내용을 주세요" 하면,

서버는 그 요청을 받아서, HTML, 이미지 등 필요한 파일을 응답(Response)으로 돌려준다.

서버는 보통 24시간 켜져 있으며, 하나의 서버가 수많은 클라이언트 요청을 처리함

## 웹 작동 흐름
1. 사용자가 브라우저 주소창에 URL 입력
2. 브라우저(Client)가 HTTP 요청을 서버로 보냄
3. 서버가 요청된 HTML 파일을 응답으로 보냄
4. 브라우저가 HTML 해석 → 사용자에게 웹페이지 보여줌


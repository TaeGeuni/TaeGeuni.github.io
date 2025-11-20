---
title: "Hugo와 GitHub Pages로 나만의 개발 블로그 만들기"
description: "Jekyll보다 빠른 Hugo, 그리고 무료 호스팅 GitHub Pages를 이용하여 깔끔한 개발 블로그를 구축하는 과정을 정리했습니다."
date: 2025-11-20T14:30:00+09:00
image: 
math: false
license: 
hidden: false
comments: true
draft: false
categories:
    - Tutorial
tags:
    - Hugo
    - GitHub Pages
    - Blog
    - CI/CD
---

개발자로서 나만의 기술 블로그를 갖는 것은 지식을 정리하고 공유하는 데 큰 도움이 됩니다. 티스토리나 벨로그 같은 좋은 플랫폼도 많지만, 커스터마이징이 자유롭고 내 데이터를 내가 온전히 소유할 수 있는 **GitHub Pages**를 선택했습니다.

그중에서도 가장 빠르고 인기가 많은 정적 사이트 생성기인 **Hugo**를 사용해 블로그를 구축한 방법을 소개합니다.

## 1. 왜 Hugo인가?

* **압도적인 속도:** Go 언어로 작성되어 빌드 속도가 타의 추종을 불허합니다. 글이 수천 개가 되어도 순식간에 빌드됩니다.
* **간편한 설치:** 의존성 설치가 복잡한 다른 툴과 달리, 바이너리 파일 하나만 있으면 설치가 끝납니다.
* **강력한 테마 생태계:** 개발자들에게 인기 있는 깔끔한 테마가 정말 많습니다.

## 2. 준비물

* GitHub 계정
* Git 설치
* Hugo 설치 (Extended 버전 권장)
* VS Code (또는 좋아하는 에디터)

## 3. Hugo 설치 및 사이트 생성

먼저 로컬 컴퓨터에 Hugo를 설치합니다. (Windows 기준)

```bash
choco install hugo-extended -confirm
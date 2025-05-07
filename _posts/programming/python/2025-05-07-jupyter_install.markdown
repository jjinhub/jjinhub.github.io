---
layout: post
related_posts:
title:  "Jupyter Notebook / Jupyter Lab 설치하기"
date:   2025-05-07 11:00:00 +0900
categories: 
  - programming
  - python
image : 
  path : /assets/img/blog/programming/python/250507_jupyter_install/thumbnail.jpg
---

***

* Table Of Contents
{:toc}

# 1. Jupyter Notebook과 Jupyter Lab 이란?
Jupyter Notebook과 Jupyter Lab은 모두 사용자가 다양한 프로그래밍 언어로 코드를 작성, 실행 및 공유할 수 있는 웹 기반 대화형 컴퓨팅 환경이다. 둘 다 대화형 데이터 사이언스 및 프로그래밍을 지원하는 것을 목표로 하는 오픈소스 이니셔티브인 주피터 프로젝트의 일부이다.

## 1.1. Jupyter Notebook
Jupyter Notebook은 2011년에 출시된 오리지널 웹 기반 컴퓨팅 환경이다. 유저는 라이브 코드, 방정식, 시각화 및 설명 텍스트를 결합한 문서를 만들고 공유할 수 있다. Jupyter Notebook은 단순하고 직관적인 인터페이스를 갖추고 있어 사용자가 쉽게 시작할 수 있으며, Python, R, Julia 등 다양한 프로그래밍 언어를 지원한다.

## 1.2. Jupyter Lab
Jupyter Lab은 2018년에 출시된 Jupyter Notebook의 더 발전된 버전이다. Jupyter Lab은 Jupyter Notebook보다 더 강력하고 유연한 환경을 제공한다. Jupyter Lab을 사용하면 여러 노트북, 코드 편집기 및 콘솔을 단일 작업 공간에서 진행할 수 있으므로, 복잡한 프로젝트를 보다 쉽게 작업할 수 있다. 또한, Jupyter Lab은 사용자가 환경의 기능을 정의하고 확장할 수 있는 확장 프로그램을 지원한다.

***

# 2. Jupyter Notebook과 Jupyter Lab의 차이
## 2.1. 인터페이스

|항목|Jupyter Notebook|Jupyter Lab|
|:---|:---|:---|
|UI 구성|단일 노트북 중심|탭/패널 기반 멀티탭 인터페이스|
|파일 탐색기|단순한 파일 목록|사이드바에 탐색기, 터미널, Git 등 다양한 툴 패널 제공|
|탭 지원|한 번에 하나의 노트북|여러 노트북, 터미널, 콘솔 등 동시 오픈 가능|

## 2.2. 파일 관리 기능

|항목|Jupyter Notebook|Jupyter Lab|
|:---|:---|:---|
|탐색기 위치|브라우저 화면 왼쪽 상단|왼쪽 패널 고정|
|드래그 앤 드롭|업로드만 가능|자유로운 파일 이동 및 열기 가능|
|파일 열기|클릭 시 새 탭에서 열림|노트북, CSV, JSON 등 다양한 유형 탭으로 열림|
|파일 변경|우측 상단의 버튼으로 가능|사이드바에서 직접 변경 가능|
|파일 검색|없음|전체 프로젝트 내 텍스트 검색 가능 (Ctrl+Shift+F)|

***
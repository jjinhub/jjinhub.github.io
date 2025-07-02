---
layout: post
related_posts:
title:  "[Jupyter] Jupyter Notebook / Jupyter Lab 설치하기"
date:   2025-07-02 11:00:00 +0900
categories: 
  - development
  - jupyter
image : 
  path : /assets/img/blog/development/jupyter/250702_jupyter_install/thumbnail.jpg
---

***

* Table Of Contents
{:toc}

# 1. Jupyter Notebook과 Jupyter Lab 이란?
Jupyter Notebook과 Jupyter Lab은 모두 사용자가 다양한 프로그래밍 언어로 코드를 작성, 실행 및 공유할 수 있는 웹 기반 대화형 컴퓨팅 환경입니다. 둘 다 대화형 데이터 사이언스 및 프로그래밍을 지원하는 것을 목표로 하는 오픈소스 이니셔티브인 주피터 프로젝트의 일부입니다.

## 1.1. Jupyter Notebook
Jupyter Notebook은 2011년에 출시된 오리지널 웹 기반 컴퓨팅 환경입니다. 유저는 라이브 코드, 방정식, 시각화 및 설명 텍스트를 결합한 문서를 만들고 공유할 수 있습니다. Jupyter Notebook은 단순하고 직관적인 인터페이스를 갖추고 있어 사용자가 쉽게 시작할 수 있으며, Python, R, Julia 등 다양한 프로그래밍 언어를 지원합니다.  

![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_01.jpg)

Jupyter Notebook 인터페이스
{:.figcaption}

## 1.2. Jupyter Lab
Jupyter Lab은 2018년에 출시된 Jupyter Notebook의 더 발전된 버전입니다. Jupyter Lab은 Jupyter Notebook보다 더 강력하고 유연한 환경을 제공합니다. Jupyter Lab을 사용하면 여러 노트북, 코드 편집기 및 콘솔을 단일 작업 공간에서 진행할 수 있으므로, 복잡한 프로젝트를 보다 쉽게 작업할 수 있습니다. 또한, Jupyter Lab은 사용자가 환경의 기능을 정의하고 확장할 수 있는 확장 프로그램을 지원합니다.  

![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_02.jpg)

Jupyter Lab 인터페이스
{:.figcaption}

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

# 3. Jupyter Notebook / Jupyter Lab 설치 및 실행
✨ **Windows 기준으로 설치 및 실행 방법을 작성하였습니다.** ✨

## 3.1. Python 설치
먼저, Python이 설치되어 있는지 확인해야합니다. 명령 프롬프트(`Win키 + R` > `cmd` 입력)를 열고 `python -V`를 입력했을 때 아래와 같이 Python 버전이 표시된다면 Python이 이미 설치된 것이고, 그렇지 않다면 Python을 설치해야합니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_03.jpg){: width="80%" height="80%"}
  
Python을 설치해야한다고 가정하고, Python 공식 웹사이트의 [다운로드 페이지](https://www.python.org/downloads/)에서 Python 설치에 필요한 파일을 다운로드합니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_04.jpg){: width="80%" height="80%"}
  
다운로드한 설치 파일을 실행하고, **Add Python.exe to PATH** 옵션을 체크합니다. 옵션을 체크해야 별도의 환경 변수 설정이 필요없습니다.  
그 다음, **Install Now**를 클릭하여 설치하고, 설치가 완료되면 **Close**를 클릭하여 창을 닫아줍니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_05.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_06.jpg){: width="80%" height="80%"}
  
다시 명령 프롬프트에서 `python -V`를 입력해보면 설치한 Python 버전이 뜨는 것을 확인할 수 있습니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_03.jpg){: width="80%" height="80%"}

## 3.2. Anaconda 설치
여기서 바로 Jupyter를 설치할 수도 있지만, 다양한 프로젝트 관리를 위한 가상환경을 사용하기 위해 **Anaconda**를 이용한 Jupyter 설치 방법을 안내해드리겠습니다.
  
Anaconda 공식 웹사이트의 [다운로드 페이지](https://www.anaconda.com/download/success)에서 OS 및 원하는 버전에 맞는 설치 파일을 다운로드합니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_07.jpg){: width="80%" height="80%"}
  
아래와 같이 옵션을 체크하고 설치를 완료합니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_08.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_09.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_10.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_11.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_12.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_13.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_14.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_15.jpg){: width="80%" height="80%"}

## 3.3. 바로가기 생성
Jupyter를 사용하기 위한 설치는 모두 끝이 났고, 실행할 때마다 명령어를 입력할 필요없이 편하게 실행할 수 있도록 바로가기를 생성하겠습니다.
  
Anaconda 설치 경로에 있는 Scripts 폴더에 들어가보겠습니다.  
예시 경로 : `C:\Users\USER\anaconda3\Scripts`
  
폴더 내에 있는 `jupyter-notebook.exe`와 `jupyter-lab.exe` 중 사용을 원하는 파일의 바로가기를 생성합니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_16.jpg){: width="80%" height="80%"}
  
그 다음, 파일을 우클릭 후 속성에 들어가 시작 위치를 지정해야하는데  
쉽게 말해 프로젝트 폴더 경로를 지정하는 과정입니다.  
Jupyter를 실행했을 때, 기본으로 시작되는 경로라 생각해주시면됩니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_17.jpg){: width="80%" height="80%"}
  
이대로 사용해도 문제는 없지만, 디테일을 살리고 싶으면 아이콘 변경을 해주시면됩니다.  
아이콘 변경 버튼을 클릭 후, Anaconda 설치 경로에 있는 Menu 폴더에 들어가 `jupyter.ico`을 적용해주세요.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_18.jpg){: width="80%" height="80%"}
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_19.jpg){: width="80%" height="80%"}

## 3.4. Jupyter 실행
모든 과정이 완료되었다면, 생성한 Jupyter 아이콘을 클릭해 Jupyter를 실행합니다.  
Jupyter가 실행되면 전 단계에서 설정했던 기본 경로가 나오고, `New` 버튼 혹은 `+` 버튼을 클릭하여 노트북, 콘솔, 터미널 등을 사용할 수 있습니다.  
  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_20.jpg){: width="80%" height="80%"}  
![](/assets/img/blog/development/jupyter/250702_jupyter_install/img_21.jpg){: width="80%" height="80%"}
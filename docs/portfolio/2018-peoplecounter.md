---
layout: default
title: People Counter, 2018
parent: Portfolio
nav_order: 6
---


## People Counter System Frontend and Hardware Interface, 2018
    1) Frontend(Angular6+)
    2) Hardware Interface(C++, Windows)
  
May 2018 ~ Apr 2019
Called people counter. In this system, there are 3 main parts, camera sensor, data processor and user interface. I actually re-developed user interface for meeting customers' evolving requrirements for data analysis for people in/out count in a building.
The basic purpose of the people counting system is as follows.

“Aggregating people entering and leaving a building or an area to create data that can be used for analytics tailored to customer needs.”

The people counting system basically consists of a camera sensor that recognizes and counts the direction of movement of an actual person, a data processing process that connects to the camera sensor and reads and stores data in a database, a web server that reads and provides data requested through the user interface, and a web client that processes the read data and displays it to user. Customer also can add more interface for storing data to another location. There are some subsidiary processes too. 
It was copy software from existing one but I can value it has infinite possibility to be developed compared to existing package.
DBMS was choosed to SQLite3 because there are no many users and I had not used this technology before. But even though concurrent users are less than 5, SQLite just allows one user at once and the data read/write rate was high, I had to be very careful to aviod racing between threads.

This system was delivered with 1 year warranty contract to
- E Mart: Simple version(planned to install 150 buildings)
- Starfield City: Advanced version (Analysis function add for by Period, Group)

[Korean]
2018년 5월 ~ 2019년 4월
기존에 개발되어 사용중인 카메라 센서 + 데이터 처리 프로세스 + 사용자 인터페이스중 카메라 센서를 제외한 데이터 처리, 사용자 인터페이스를 진화하는 고객 요구사항에 맞게 지속적으로 개선하기 위한 작업으로, 같은 기능의 프로그램을 향후에 발생할 요구사항에 적극 대응하기 위해 (기존 하드웨어 회사의 기본 프로그램을 대체하는 형태로 다시) 개발하였다.
피플카운팅 시스템의 기본 목적은 다음과 같다.

“건물 또는 어떤 구역에 들어오고 나가는 사람들을 집계하여 고객이 원하는 용도에 맞게 분석하는데 쓰일 데이터를 만듬.”

피플카운팅 시스템은 기본적으로 실제 사람의 이동 방향을 인지하고 집계하는 카메라 센서, 카메라센서에 접속하여 데이터를 읽어와 데이터베이스에 저장하는 데이터 처리 프로세스, 사용자 인터페이스를 통해 요청된 데이터를 읽어서 제공하는 웹 서버, 읽어들인 데이터를 가공하여 웹페이지에 표출하는 웹 클라이언트로 구성하며, 필요에 따라 외부 데이터베이스에 접속하여 보유한 데이터를 원하는 형태로 저장하는 역할을 하는 인터페이스를 추가한다. 이 외에도 파일 로깅 등의 부수적인 역할을 담당하는 프로세스도 있다.
이미 만들어진 소프트웨어의 카피 형태이지만 기존 소프트웨어 패키지에 비해 발전 형태가 무궁무진하다는 점에서 의의를 두겠다.
DBMS는 Sqlite로 선택하였는데, 어플리케이션 사용자가 많지 않고, 사용해보지 않았던 기술이라 겸사겸사 적용해보았다. 다만 사용자가 5명 이내로 많지 않은 어플리케이션임에도 불구하고 Sqlite가 한 번에 하나의 접속만을 허용하는 DB이고, 수시로 읽고 쓰는 데이터량이 많다보니 프로세스, 스레드간의 경합(DB접근)을 매우 주의해서 코드를 작성해야만 했다.

해당 시스템은 다음의 회사에 시스템 판매(1년 무상 기술지원) 형태로 납품하였다.
    - 이마트: 단순한 데이터 처리, 표출만을 위한 버전(약 150개 점포 설치(예정))
    - 스타필드시티: 기간, 그룹별 분석 기능을 추가한 버전

![sample img](/assets/images/portfolio-2017-lms.jpg)

- Developer: Taeung Ha
- Actual time for development: about 3 months for core part
- Contribution rate: 100%
- Technologies used: Angular6+, C++(boost beast), Http, WebSocket, SQLite
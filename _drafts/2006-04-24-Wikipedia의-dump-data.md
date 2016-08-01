---
layout: post
title: "Wikipedia의 dump data"
date: 2006-04-24 21:24
categories: ⊙ 전공노트
---

http://download.wikimedia.org/

DataMing이라는 녀석을 Wikipedia에서 검색하기 위해 http://en.wikipedia.org/Data_Mining 을 주소창에 입력하고 엔터를 치는 순간, 갑자기 에러 페이지가 뜨면서 http://download.wikimedia.org/ 라는 녀석을 방문해보라고 가르쳐줬다. 웬 황당한!

그것 참, 요즘 사회연결망연구라는 김용학 선생님 수업을 들으면서 Wikipedia를 분석해보려고 이런 저런 고민을 하고 있었는데, 그 중 가장 큰 고민이 이거였다. 그 엄청나게 많은 Wikipedia의 데이터들을 어떻게 추출할까? 전체 index를 다 볼 수 있는 메뉴가 있을까? 그 index들을 따라 http 요청을 하게 되면 서버에 너무 많은 부하를 주지 않을까? IP ban 당하는건 아닐까?

이런 저런 고민들이 정말 황당한 순간에 모두 해결되는 순간이었다. Wikipedia의 모든 컨텐츠들은 GFDL(GNU Free Documentation License)를 따르며, 그 데이터들을 모두 http://download.wikimedia.org/ 이 녀석에서 다운받을 수 있는 것이었다! 완전!

http://meta.wikimedia.org/wiki/Data_dumps 에서 좀 더 자세한 설명을 볼 수 있다.

Dump에서 제공하는 정보는
Page contentPage-to-page link lists (pagelinks, categorylinks, imagelinks tables)Image metadata (image, oldimage tables)Misc bits (interwiki, site_stats tables)랜다.

연구해보려는 주제에서 history 정보도 필요하긴 한데, 영문 wikipedia의 경우는 파일이 너무 커서 current page contents만 제공한다고 한다. current version만 텍스트 압축률이 타의 추종을 불허하는 bzip2로 압축된 xml 크기만 1.9GB다. 이거 풀면 20~100배 정도 커진다고 한다. 세상에 raw data만 100GB짜리 데이터 구하기 정말 힘들다. 그것도 현존하는 집단지성의 최고봉인 Wikipedia의 데이터일바에야 더 할 말이 있으랴.


설마... 뒷북일까? -.-)a 

       

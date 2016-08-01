---
layout: post
title: "SourceForge project raw data"
date: 2006-04-24 23:17
categories: ⊙ 전공노트
---

내친김에 SourceForge에 등록된 프로젝트들의 리스트와 개발자, 후원자 등의 정보를 raw data로 구할 수 있는지 찾아봤다. 예전에 한 번 검색해보다가 나중으로 미뤘었는데 wikipedia dump의 발견으로 갑자기 의욕이 솟아났다.

Google에서 sourceforge data로 검색했더니, 웬걸, 예전에는 잘 안보이던 링크가 보였다. [http://www.nd.edu/~oss/Data/data.html](http://www.nd.edu/%7Eoss/Data/data.html) 노틀담 대학이 학술 목적으로 SF.net에게 제공받은 데이터를 연구용으로 열람할 수 있도록 해주나보더라. 

또 하나 더, FLOSSmole([http://ossmole.sf.net/](http://ossmole.sf.net/))이라는 녀석. SourceForge에 하나의 프로젝트로 등록되어있는 녀석이었다. 전체 프로젝트 리스트인지는 모르겠지만, 2005년 4월부터 매달마다의 프로젝트 리스트, 프로젝트 설명, 개발자, 후원자 등의 정보를 업데이트해오고 있다. 아카이브 용량이 꽤 많이 들텐데 어떻게 감당하고 있는건지 원. 

하지만 슬프게도 이 사이트에 이미 선행 연구가 게제되어 있었네. SF.net에 대한 네트워크 분석의 첫 타자는 놓친듯 하다. 

[Howison, J., Inoue, K., and Crowston, K. (2006). Social dynamics of free and open source team communications. In Proceedings of the IFIP 2nd International Conference on Open Source Software, Lake Como, Italy. Available from: http://floss.syr.edu/publications/howison_dynamic_sna_intoss_ifip_short.pdf](http://floss.syr.edu/publications/howison_dynamic_sna_intoss_ifip_short.pdf)

라는 녀석이란다. 흑, 2006년 연구라니. 좋은 연구 주제인 것 같다. 나도 개발자를 매개로 프로젝트들간에 어떤 관계가 있는지 조사해볼까 했는데, 내가 구상했던 것보다 더 세련된 연구주제인 듯 하다. 프로젝트 description을 context analysis해서 어떤 키워드가 기부(donation)를 많이 받는지 한 번 연구해보고 싶은데... 이 연구에 사용된 intermediate data (in the form of R)와 논문의 latex 파일을 제공한다고 한다. ([link](http://ossmole.sf.net/2006/03/social-network-analysis-over-time.html)) 

현재 날짜까지의 데이터로 분석한 몇 가지 흥미로운 결과들도 게시해 놓았다. ([link](http://http://ossmole.sf.net/2006/02/some-pretty-pictures-to-amuse-you.html)) 가장 연결이 많이 되어있는 개발자는 [Nupur Sarpal](http://sourceforge.net/users/saunup/)이라는 사람이랜다. 이 사람의 분야는? 재밌게도 디자이너랜다. 하핫, 이거야말로 네트워크 분석의 재미있는 점이 아니겠는가? 한국 영화배우 네트워크에서 박용팔씨가 중앙에 위치하게 된 것처럼, 네트워크에서 중앙에 위치하게 되는 사람은 우리가 예전에 생각하던 권력(Power)을 가진 사람으로 해석하면 안되는 것이다. 나조차 저 통계를 보면서 기대했던건 뭔가 경력있고 실력있는 개발자가 나타나는 것이었단말이다! 이런 통념을 무참히 깨버리는 결과라니, 머리를 시원하게 해버리는걸?

[http://libresoft.urjc.es/Data/CVSAnalY_SF](http://libresoft.urjc.es/Data/CVSAnalY_SF) 허헛, 이거야 원 여기서도 SF.net에 대한 뭔가 분석을 했었나보다. 이거 뭐야, 되게 많네;; [http://libresoft.urjc.es/Results/index_html](http://libresoft.urjc.es/Results/index_html) KDE, GNOME, Debian 등의 CVS를 계속 모니터링하면서 분석하고 있다보다.

그러고보니 Ubuntu package에서 package간의 의존관계를 SNA로 분석해보는 것도 재밌을 것 같다. 그러면 이건 도대체 무슨 분야의 연구가 되는거지? 

       

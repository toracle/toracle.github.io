---
layout: post
title: "Sun Microsystems은 무슨 생각을?"
date: 2005-06-16 00:40
categories: ⊙ 전공노트
---

Sun에서 계속 Solaris을 홍보하는 메일이 온다. (메일링 리스트에 가입되어 있으니 당연한 일이지만.)
요즘 메일 내용의 80%는 Open Solaris 10에 대한 내용이라고 해도 과언이 아니다.
얼마 전에는 I Love Solaris 공모전도 개최했는데, 신청자가 적다고 무료 세미나도 초대하고 마감 기한도 연장하고 그러더라.

하지만 Sun도 수익을 남겨야 하는 회사인데, 과연 어떤 전략을 가지고 있는것일까?

Sun에서 Solaris10 이외에 가장 주력하고 있는 분야는 단연 Java일 것이다. 하지만 J2SE, J2EE 역시 (Sun 홈페이지의 표현에 따르면) free이다. Application Server도 free이고, SunONE Directory Server도 free이다. 과연 Sun은 뭘 먹고 살려는 것이지?

조엘 온 소프트웨어의 한 쳅터에 있던 무슨 기법이더라, 간단한 경제학 기법이라고 소개했었는데, 그걸 토대로 이야기를 풀어보면.

Sun은 하드웨어 회사다. x86 기반 Solaris를 내놓았지만 아직도 SPARC 기반 소프트웨어들이 많고, 관련 웍스테이션, 서버 제품군도 많다. 그렇기 때문에 Sun은 Solaris와 J2SE, J2EE 등을 무료로 공급하면서 SPARC으로 진입하기 위한 장벽을 낮춤으로써 SPARC의 판매 증진을 노리려는 것이다.

라는 생각을 하나 해볼 수 있다. 

참, 비슷한 맥락으로, Java Studio Creator나 Java Studio Enterprise 등은 꽤 비싸다(지금 대학생 신분으로 느끼기에는). 특히 J2EE 같은 경우 Sun의 구현이 가장 보편화되어 있고, Application Server 등과 연동하기 위해서는 아무래도 Java Studio Enterprise 등이 편리한 환경을 제공할 것이다. 그렇다면 Java를 보급시킴으로서 Java 개발도구를 판매하려는 의도인가?

뭐 결론이 날 이야기는 아닌 것 같고.

하여튼 Sun이 Java에 이어 Solaris 10도 성공시키려고 안간힘을 쓰고 있는 것 같다. 물론 전산학자들의 향수 속에는 SunOS, Solaris에서 보여준 혁신의 이미지가 남아있겠지만, 사용자의 입장에서 Solaris 10은 아직 데스크탑으로서는 미숙한 OS라고 보여진다. 터미널 기반도 아니고 - 기본으로 설치되는 쉘이 csh였던걸로 기억한다. tcsh나 bash도 아니고 - 완전한 GUI 기반도 아닌 것이, 또 사용자 계정도 root 기반으로 되어 있고, /usr, /usr/home, /etc 등의 전통적인 유닉스 디렉토리 구조를 갖춘 멀티 유저 환경을 one 유저 환경으로 사용한다는 것도 관리하기가 참 애매하다.

Sun의 제품군들을 전체적으로 보고 있노라면, Java와 Solaris 기반으로 thin client 환경을 구상하는 것 같은데, 뭔가 서로 아귀가 맞지 않는듯한 느낌이다. 잘 파악을 못해서 그런가? 그냥 느낌상으로는 MS보다는 Sun이 신뢰가 가는데, 제품군도 Sun에서 말하는 것처럼 그렇게 저렴한 것 같지도 않고 - Sun Ray Thin-Client 1g 한대에 35만원 정도 하는 것 같다. 웬만한 P-4 2.4GHz Fat client를 비슷한 가격에 구입할 수 있는 것을 생각하면 그렇게 큰 메리트가 있는 것 같지 않다. 참, Fat client - Windows 환경은 OS 가격 최소 20만원을 덧붙여야 하는거군.

무슨 생각을 하는걸까?

Sun 솔루션이 구축된 환경을 직접 볼 수 있었으면 좋겠는데...

       

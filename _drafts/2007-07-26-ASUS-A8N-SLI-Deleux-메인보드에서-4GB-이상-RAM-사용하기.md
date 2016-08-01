---
layout: post
title: "ASUS A8N-SLI Deleux 메인보드에서 4GB 이상 RAM 사용하기"
date: 2007-07-26 13:26
categories: 
---



ASUS A8N-SLI Deleux 메인보드는 램을 4GB 이상 장착할 수 있다고 설명서에 나와있다. 그러나 Windows XP SP2를 설치해보면 램이 3GB 밖에 잡히지 않는 것을 볼 수 있다.

 

분명히 BIOS에서는 Physical Memory가 4096MB라고 잡혀있는데, 윈도우에서는 3GB밖에 인식을 못하는 것이다.

 

이 문제는 Microsoft에서 KB로 제공하는 이슈이며, 해결책과 원인은 다음 URL에서 찾아볼 수 있다.

 

[http://support.microsoft.com/?id=888137](http://support.microsoft.com/?id=888137)

 

요지는 4GB 이상의 램을 지원하는 PAE 모드 작동방식이 SP2에서는 바뀌었다는 것인데, boot.ini에 /pae 파라메터를 더해줘야 한다.


       

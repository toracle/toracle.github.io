---
layout: post
title: "Recovery Kit"
date: 2006-02-17 22:41
categories: ⊙ 전공노트
---

지난 몇년간 해외에서 PC 수리를 하러 다닐 기회가 종종 있었다. 

당연히 고장 원인은 하드웨어 아니면 소프트웨어이겠지. 하드웨어의 경우는 그다지 손볼 여지가 없다. 그저 부품 청소해주고 CPU부터 다시 조립해보는 정도? 기계적으로나 전기적으로 못쓰게 된 부품들은 솎아내는 것 이외에는 손댈 수가 없다.

관건은 소프트웨어의 경우이다. 이 경우는 OS를 뒤엎어서 해결하게 될 때가 많다. 그런데 그러려면 데이터를 백업해놓아야 한다. 그러면 데이터를 어디에다가 백업해놓아야 할까? 파티션이 나누어져 있는 경우라면 다른 파티션에 옮겨놓으면 될테고, 그렇지 않다면 하드를 붙여다가 복사를 하거나 외장 하드 케이스를 연결해서 복사를 하면 된다. 그 다음이야 일사천리.

자 그런데 만약 윈도우가 기동이 되는 경우라면 별 상관 없는데, 윈도우가 깨진 경우라면 문제가 좀 복잡해진다. 미리 준비해놓은 부팅 디스켓이 없는 경우가 많기 때문에 여기 저기서 부팅 디스켓을 구하러 다니거나 근처에 있는 온전한 윈도우 시스템에서 복구 디스켓을 만들어 오는 경우가 많다. 그런데 이놈의 도스는 USB나 Firewire 지원을 하지 않기 때문에 외장 하드는 사용하지 못한다. 결국 케이스를 뜯어서 하드를 붙여야 한다는 이야기.

더 골때리는 상황은, 파일 시스템이 NTFS인 경우이다. 이 경우에는 보통의 DOS로는 파일시스템이 읽혀지지 않는다. Windows XP 복구모드로 들어가던지 - 여기서 할 수 있는 작업은 매우 매우 제한되어 있다. 복사조차 못할걸? 결국 파일 시스템이 NTFS인 경우에는 데이터를 못살린다는 이야기이다.


그래서 매번 해외에서 돌아올 때마다 recovery kit을 제작해야겠다는 생각을 하곤 한다. 물론 매번 까먹는다.
우선 부팅 가능한 CD여야 한다. 물론 간혹가다가 CD가 없는 시스템도 있고, 구형 CD-ROM일 경우 CD를 잘 인식하지 못하는 경우도 있지만, 그런 경우는 어쩔 수 없다고 치고 - FD를 사용한 kit 버전도 생각해볼만하다. OS는 Linux여도 좋겠고, DOS여도 좋겠다. 결국 데이터를 복사할 수 있으면 되니까 Linux여도 문제는 없다.USB와 Firewire를 지원해서, 외장하드를 사용할 수 있도록 지원해야 한다.NTFS에 접근할 수 있어야 한다.이런 정도를 지원하는 솔루션들이 있는지 모르겠다. 우선 부팅 가능한 작은 Linux야 뭐 만들 수 있겠다. 그리고 DOS용 USB, Firewire 드라이버를 만들 수 있을까? 그래서 하드로 인식할 수 있도록 하는 드라이버 말이다. NTFS는 [Sysinternals](http://sysinternals.com/) 의 [NTFSDOS](http://www.sysinternals.com/Utilities/NtfsDosProfessional.html)라는 소프트웨어-DOS라는 솔루션이 있다.

또 오늘 생각났는데 undelete.exe 같은 간단한 프로그램이라도 있어야 하지 않을까? FinalData 같은 거대한 프로그램이 아니더라도, 300KB짜리 작은 복구 프로그램도 있더라. 그 정도는 만들어서 쓸 수 있지 않을까?

여튼 언젠가 저런 Kit를 만들던지, 다른 누군가가 잘 만들어서 해외 PC 수리 출장을 흡족하게 성공했으면 좋겠다.

       

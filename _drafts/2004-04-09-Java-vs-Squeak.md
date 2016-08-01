---
layout: post
title: "Java v.s. Squeak"
date: 2004-04-09 20:09
categories: ⊙ 짧은 생각들
---

Java가 등장한 것은, machine independent한 language를 만들고자 해서였다. 때문에 JVM이라는 intermediate virtual machine을 만들고 어떤 machine에서건 소스 레벨의 수정 없이 프로그램을 돌아가도록 만들었다. 그런데 그것이 오히려 Java의 최대 단점이 되었다. 편리한 OOP, 일관성있는 API 등 많은 장점이 있는데도 불구하고 Java를 기피하는 최대 원인은 Java의 최대 장점 중 하나인 platform independent를 구현하기 위한 느린 속도이다.

때문에 여러 가지 대안들이 등장했다. JIT(Just-In-Time) compiler도 그 하나의 대안이다. 그리고 그 대안들 중 하나가 아예 JVM을 virtual machine에서 real machine으로 끌어올리자는 것이다. 이른바 Java Machine인 셈이다.

하지만 과연...? 비슷한 예가 이미 있었다. SmallTalk이라는 언어에서 파생한 Squeak은 OOP를 가장 잘 구현한 언어 중 하나라는 극찬을 받았지만, (어떤 이유에서인지는 잘 모르겠지만) 역사의 뒤안길로 사라져버렸다. 그리고 그 Squeak은 Squeak Machine을 가지고 있었다. 하지만 개인적인 생각으로는 오히려 그것이 제약이 된 것 같다. Squeak이라는 편리한 authoware가 있었지만, 오직 그것만 사용해야 한다는 것이 맹점이었던 것 같다.

GNUstep 역시 주 언어는 Objective-C인데, 여러 platform에서 돌아가는 platform이면서도 Objective-C를 주로 사용한다는 것이 오히려 제약이 될 수도 있을 것 같다.

Java Machine이 과연 실용화될지, 그리고 얼마나 호응을 얻을지는 잘 모르겠지만, Squeak machine과는 다른 길을 걷게 된다면 역사의 아이러니가 아닐 수 없다.

       

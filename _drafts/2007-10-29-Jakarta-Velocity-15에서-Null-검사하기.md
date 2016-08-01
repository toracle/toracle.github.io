---
layout: post
title: "Jakarta Velocity 1.5에서 Null 검사하기"
date: 2007-10-29 10:30
categories: ⊙ 전공노트
---



Velocity의 VTL에서 종종 변수에 들어있는 값이 null인지 검사해야 할 경우가 생긴다.

예를 들어 

> #if ($myvar == null)
    I am null
#else
    I am not null과 같은 조건을 사용해야 할 경우이다.

하지만 위와 같이 템플릿을 작성하게 되면 velocity가 Null Reference Exception을 내면서 죽어버린다.
Velocity가 null을 참조하게 되면 문제가 생기는 모양이다.

이런 경우에는 다음과 같이 변수의 값을 체크해야 한다.
> #if (!$serialnum && "$!serialnum" == "")이렇게 사용하면 변수의 값이 null인지 여부를 체크할 수 있다.

더 자세한 내용은 velocity wiki 페이지인 [http://wiki.apache.org/velocity/CheckingForNull](http://wiki.apache.org/velocity/CheckingForNull) 를 참조.
       

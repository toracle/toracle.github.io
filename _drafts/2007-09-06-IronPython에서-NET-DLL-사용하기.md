---
layout: post
title: "IronPython에서 .NET DLL 사용하기"
date: 2007-09-06 20:41
categories: 
---



IronPython은 .NET으로 만들어진 Python 클론이다. Jython이 Java와의 바인딩이 자유자재인 것처럼 IronPython도 .NET으로 만들어진 프로그램들을 자유자재로 가져다 사용할 수 있다.




요즘 회사에서 만들고 있는 알고리즘 모듈을 C#으로 작성하고 있다. 그런데 이 녀석이 여러 알고리즘 모듈을 한꺼번에 사용해야 할 경우가 많아서 임시방편으로 DOS BATCH를 사용해 돌리곤 하지만, 조금 복잡한 작업을 해야 할 경우는 새로 유틸리티를 만들어야 한다. 이러던 참에 IronPython을 사용해볼까 하고 알아봤는데, 기본적인 DLL 로딩 방법도 모르겠더라.

인터넷에서 조금 찾아보니 다음과 같은 코드를 사용하면 .NET 어셈블리를 가져다 쓸 수 있다는걸 발견했다. 퍼포먼스가 필요한 엔진은 C#이나 C++로 모듈화해놓고, IronPython으로 가져다 쓰면 편하겠다. CPython처럼 (자세히 살펴보지는 않았지만) 복잡한 API를 구현하지 않아도 돼서 편하다.

다음은 IronPython에서 .NET 어셈블리 DLL을 로딩하여 클래스를 사용하는 코드의 예이다.



> 

import clr
clr.AddReference('Algorithms.DLL') 



import MyProgram
import MyProgram.Algorithms
import MyProgram.ModLocalizer as ModLocalizer
import MyProgram.Logger as Logger 



import System.Console as Console 



m = ModLocalizer('D:\\Cyram Work\\MyProgram100_nodes_rgg.mod')
l = Logger(Console.Out, Console.Out)
m.AddLogger(l) 



m.Run()


       

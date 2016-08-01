---
layout: post
title: "Eclipse 3.2.x에서 Subclise 설치하기"
date: 2007-07-22 20:25
categories: ⊙ 전공노트
---

CVS 이후 등장한 코드 관리 시스템으로 주목받고 있는 서브버젼 - Subversion(줄여서 SVN)을 이클립스에서 사용하기 위해서는 별도의 플러그인을 설치해야 한다. 이클립스용 서브버전 플러그인에는 여러 가지가 있지만, 이 아티클에서는 Subclipse라는 플러그인을 설치하는 방법을 소개한다.

Subclipse의 공식 홈페이지는 [http://subclipse.tigris.org](http://subclipse.tigris.org)이다. 하지만 이클립스에서 설치할 때는 공식 홈페이지를 방문하지 않고도 이클립스의 업데이트 기능을 이용해서 설치할 수 있다.

[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_07072926.png]이클립스를 처음 실행했을 때의 화면이다.
[http://thumbnail.egloos.net/600x0/http://pds5.egloos.com/pds/200707/22/66/a0006366_07070159.png]Help -> Software Updates -> Find and Install 항목을 선택한다.

[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_07075456.png]위와 같은 위저드 페이지가 뜬다. 아랫쪽의 Search for new features to install을 선택하고 Next 버튼을 누른다.

[http://thumbnail.egloos.net/600x0/http://pds5.egloos.com/pds/200707/22/66/a0006366_07073259.png]업데이트 정보가 존재하는 사이트들의 목록이 나타난다. Subclipse 플러그인을 제공하는 사이트는 기존에 존재하지 않으므로 목록 오른쪽편의 New Remote Site를 클릭한 후 위와 같은 입력창을 띄운다.

[http://thumbnail.egloos.net/600x0/http://pds5.egloos.com/pds/200707/22/66/a0006366_0707574.png]Name에는 사용자가 식별할 수 있는 이름을 적고, URL에는 http://subclipse.tigris.org/update_1.2.x 를 적는다. (Eclipse 3.2.x 버전일 경우 해당한다. Eclipse 3.1.x나 3.0.x를 사용하는 경우는 http://subclipse.tigris.org/update_1.0.x를 적어주면 된다.)


[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_07075320.png]위와 같이 Subclipse의 업데이트 사이트가 등록되었다면, Finish 버튼을 눌러 업데이트할 요소들을 확인한다.

[http://thumbnail.egloos.net/600x0/http://pds5.egloos.com/pds/200707/22/66/a0006366_07074469.png]이클립스가 업데이트 사이트에 접속하여 설치할 항목들을 확인한다.[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_07072252.png]Subclipse에 해당하는 항목들이 보여진다. 최상위의 Subclipse 폴더를 펼쳐보면 두 가지 항목을 설치할 수 있는데, 위의 Integration은 선택을 해제한다. Next를 누른다.

[http://thumbnail.egloos.net/600x0/http://pds4.egloos.com/pds/200707/22/66/a0006366_08075997.png]Subclipse의 라이센스를 보여준다. 라이센스에 동의하면 Next 버튼이 활성화된다.

[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_08074546.png]설치할 항목을 다시 확인한다. Finish 버튼을 누르면 사이트로부터 다운로드를 시작한다.

[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_08073956.png]이클립스가 사이트로부터 설치할 파일을 받기 시작한다.

[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_0807226.png]다운로드 받은 파일을 설치할 것인지 다시 한 번 확인한다. Install All을 클릭해준다. 

[http://thumbnail.egloos.net/600x0/http://pds3.egloos.com/pds/200707/22/66/a0006366_08073816.png]설치가 완료되면 이클립스를 재시작해야 한다. Yes 버튼을 눌러 이클립스를 재시작한 이후부터는 Subclipse가 동작할 것이다.

       

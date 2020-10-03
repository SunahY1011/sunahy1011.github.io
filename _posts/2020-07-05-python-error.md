---
title: "그동안 겪었던 Python 관련 error 모음"
excerpt: "python을 쓰기 위한... 노오력...."

categories: 
    - python
tags:
    - python
    - error
last_modified_at: 2020-07-05T08:06:00-05:00
---

앞으로 발생하는 모든 python error를 해결하고 정리해보자ㅠㅠㅠㅠㅠ  
한참 찾았지만, 아주 별거 아닌 이유로 해결되는 문제들 모음임 ^ㅅ^ 
  
참고) OS : Windows10

### system error code 193
  
Update : 2020.07.05  

%1은(는) 올바른 win32 응용 프로그램이 아닙니다  
%1 is not a valid Win32 application  
  
위와 같은 에러가 나왔다.  
기존에는 아무런 문제가 없었는데 갑자기 이런 에러가 생겼다.  
똑같이 가상환경에서 Django를 실행하고 app을 만드는데, 이전에 만들어뒀던 상황에서는 문제없이 startapp이 작동하고, 새로 만든 가상환경에서는 작동하지 않았다.ㅠㅠ  
  
**결론) 가상환경을 만든 python이 32bit인지 64bit인지에 따른 차이**   
  
작동하는 가상환경을 만들었을 때 python을 실행하면  
Python 3.7.3 (v3.7.3:ef4ec6ed12, Mar 25 2019, 21:26:53) [MSC v.1916 32 bit (Intel)] on win32 와 같이 나오고  
  
작동하지 않는 가상환경을 만들었을 때 python을 실행하면  
Python 3.7.1 (default, Dec 10 2018, 22:54:23) [MSC v.1915 64 bit (AMD64)] :: Anaconda, Inc. on win32 와 같이 나온다.   
  
중요한 차이는 **[MSC v.1916 32 bit (Intel)] vs [MSC v.1915 64 bit (AMD64)]**에 있다.  

이를 확인하는 방법은 cmd 창에서 python을 실행해보면 안다.

![](https://sunahy1011.github.io/assets/images/0705pythonerror(1).JPG){: .align-center}
  
나는 전자가 필요했고, 이를 수정하는 방법은 두 가지였다.  
1) 환경변수 설정  
2) python 최신버전을 또 설치하는데 이때 이전 버전을 지울 필요는 없고, 조심할 것은 **32bit** 를 다운받아 설치해야한다.  

두 번째 방법을 실행!

그리고 나서 다시 cmd 창에서 똑같이 확인해보면 바뀐 것을 확인할 수 있다!!!!

이거 해결하는데 3시간 걸렸다!!!!

----
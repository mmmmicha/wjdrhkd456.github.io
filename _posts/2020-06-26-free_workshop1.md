---
title: "Free workShop 1번 - HttpSession 과 @SessionAttributes"
date: 2020-06-26 23:56:00 -0400
categories: session @SessionAttributes HttpSession
---

오늘은 제가 예전부터 궁금했던 **session** 에 대한 **무기한 workshop** 을 열어두려고 합니다. ~~workshop은 공동작업공간이라는 의미로 사용했습니다.~~<br><br>

session이란 무엇인가..<br><br>

> session : 네트워크 분야에서 반영구적이고 상호작용적인 정보 교환을 전제하는 둘 이상의 통신 장치나 컴퓨터와 사용자 간의 대화나 송수신 연결상태를 의미하는 보안적인 다이얼로그 및 시간대

<br><br>평상시 사용하던 session을 사전적인 의미로 보니 굉장히 낯선데요, 주목해볼 부분은 **반영구적** 이면서 **상호작용적인 정보교환을 전제하는** 인 것 같습니다.<br><br>

Web Backend(ServerSide)에서의 session은 server의 메모리에 데이터를 저장하는 용도로 사용합니다.<br>
server의 메모리를 사용하면서까지 데이터를 저장하는 이유는 아주 큰 장점 때문입니다.<br>
그것은 바로 server의 메모리에 잘 보관되고 있는 정보를 다양한 상황에서 언제든(?) 꺼내서 쓸 수 있다는 점입니다. ~~protocol을 통해 주고 받게 되겠지만 이렇게 얘기하겠습니다~~<br>
이는 웹 어플리케이션에서 진가를 발휘하게 됩니다. <br>
가장 보편적인 예로, 로그인 시 사용자들의 식별 정보를 session에 담고 이를 통해 user에게 알맞는 서비스를 제공해줄 수 있습니다.<br><br>

이제서야 얘기하게되는 이번 workshop에 등장하는 두 키워드 **HttpSession** 과 **@SessionAttributes** 는 session을 사용하기 위한 api입니다.<br>
HttpSession과 @SessionAttributes 는 가장 큰 차이점을 가지고 있습니다.<br>
HttpSession은 Controller를 넘나들며 사용을 할 수 있지만, @SessionAttributes는 @Controller가 명시된 해당 클래스 내에서만 데이터 공유가 이루어 진다는 것입니다.<br>
저는 두 api를 모두 사용해보면서 session을 사용하는 대부분의 취지엔 HttpSession이 맞겠다고 생각을 하고 있습니다.<br><br>

한 class내에 국한되는 **@SessionAttributes** 의 장점은 무엇인지, 제가 혹시 이 api를 광범위하게 사용하는 방법을 모르고 있는건지 ~~googling을 충분히 했다고 생각하는데 아직까진 발견하지 못했습니다..~~<br>
이 workshop에 자유롭게 의견을 남겨주시면 감사하겠습니다!

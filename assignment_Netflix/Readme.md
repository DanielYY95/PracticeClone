<HTML 설계>

1. Header부분: 왼쪽 Netflix 로고, 오른쪽에 언어 toggle(button), 로그인 button
2. h1, h4, h6
3. Input창 + button과 enter
4. 배경화면 전쳬
5. footer



<에러>

1. header, footer 대신 div 로 묶어야 잘 되는 느낌
2. 뭔가 적용이 안되는가 싶으면 선택자를 살펴보기!
3. header 나 content는 안에 div가 있으면 좌우로 쫙 뻗어 있는데, footer는 왜 안 그러지....??
==> position: fixed를 쓰면 그렇게 되네...
4. height 설정을 잘 못하고있네.....
5. 쓸데없이 login 태그를 만들었더니.... 더 힘드네.. 그냥 content에 합쳤다...
6. 글짜 굵기 어떻게 못하나??
7. ::before and ::after 를 어떻게 적용해야할지?

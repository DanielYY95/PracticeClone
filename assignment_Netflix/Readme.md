<HTML 설계>

1. Header부분: 왼쪽 Netflix 로고, 오른쪽에 언어 toggle(button), 로그인 button // 반응형. position: absolute; 활용 but flex를 사용할 걸... 
2. h1, h4, h6 // flex 사용, justify 와 align-item 사용
3. Input창 + button // 반응형으로. flex와 행열 정렬 교체. justify-content: center; 
4. 배경화면 전쳬 // vw, vh 활용
5. footer // flex를 사용하고 end를 통해 맨 밑으로 배치



<에러>

1. header, footer 대신 div 로 묶어야 잘 되는 느낌
2. 뭔가 적용이 안되는가 싶으면 선택자를 살펴보기!
3. header 나 content는 안에 div가 있으면 좌우로 쫙 뻗어 있는데, footer는 왜 안 그러지....??
==> position: fixed를 쓰면 그렇게 되네...
4. height 설정을 잘 못하고있네.....
5. 쓸데없이 login 태그를 만들었더니.... 더 힘드네.. 그냥 content에 합쳤다...
6. 글짜 굵기 어떻게 못하나??
7. ::before and ::after 를 어떻게 적용해야할지?
8. line-height는 영역을 침범을 하는듯 .... 개발자도구에서 잘 살펴봐야한다. 
9. justify-content 이 작동되지않는 경우
- justify-content only has an effect if there's space left over after your flex items have flexed to absorb the free space. In most/many cases, there won't be any free space left, and indeed justify-content will do nothing.
- justify- content: center가 먹히지않는 경우,
display: flex; flex-direction: column; align-items: center; ==> 간혹, justify-content가 먹히기도 하지만, 이게 국룰이다.
- justify-content property (works on main axis only) flex-direction이 바뀌면 main axis도 바뀐다.
https://stackoverflow.com/questions/35106814/why-isnt-justify-content-centering-my-divs
====> flex로 container의 가로 세로 가운데로 배치하고 싶다면 justify-content:center와 align-items: center 모두 사용!

<개선 점>
1. absolute 하고, bottom: 0 이렇게 하는 것보다 차라리 display: flex;   justify-content: center;  이게 낫겠다. 
2. 저기 select와 로그인 button을 position: absolute 말고 div 로 묶어서 flex 해도 될듯\



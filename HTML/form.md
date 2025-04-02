form 태그는 다음과 같은 기능이 있다.

`action` 속성: 가고 싶은 주소
`method` 속성: 사용하고 싶은 방식 `GET`, `POST`

특이사항으로는, form 태그 안에 `button` 태그를 사용하게 되면 이 `button`태그는 전송 기능이 자동으로 생긴다. 만약 form 태그 안에 여러 버튼을 두게 될 경우 `<button type="button"></button>`을 사용해 일반 버튼으로 만들어야 전송 기능을 하지 않는다.
해당 페이지 주소 : https://webhacking.kr/challenge/web-01/

![image](https://user-images.githubusercontent.com/120306359/216098620-f2b5da83-c1aa-4453-86d1-293dcdac3346.png)

처음 페이지에 접속하면 다음과 같은 화면을 확인할 수 있다.

여기서 view-source를 클릭한다.

![image](https://user-images.githubusercontent.com/120306359/216098991-ab07696f-5788-4f0c-a99d-ff84badde2d4.png)

윗 부분의 php 소스는 user_lv의 쿠키 값이 존재하지 않으면 setcookie를 이용해서 설정한다는 의미이다.

아랫 부분의 php 소스는 user_lv의 쿠키 값이 4이상이면 쿠키 값을 다시 1로 설정한다.

그리고 user_lv의 쿠키 값이 3보다 클 경우에는 solve(1)을 실행한다.

따라서 user_lv의 쿠키 값은 3과 4사이의 값으로 설정해야 한다.

![image](https://user-images.githubusercontent.com/120306359/216113088-cfc2f22c-ed96-4c3b-a2f4-651a39f160c4.png)

EditThisCookie에서 user_lv의 쿠키 값을 3.5로 바꾸었다.

![image](https://user-images.githubusercontent.com/120306359/216113369-1292749c-b822-4baf-864a-2f4f8acdf0d1.png)

그리고 다시 사이트에 접속하니 문제가 해결되었음을 확인할 수 있다.

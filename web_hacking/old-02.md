해당 페이지 주소 : https://webhacking.kr/challenge/web-02/

old-02 페이지만 유독 느려서 진행하는데에 어려움이 있었다.

페이지가 열리지 않아서 일단 다른 문제부터 풀었다.

![image](https://user-images.githubusercontent.com/120306359/216117852-66f7cbc4-4496-45ba-b27b-73604c99d464.png)

처음 페이지에 접속하면 다음과 같은 화면을 확인할 수 있다.

화면 상으로는 찾을 수 있는 정보가 없어 f12를 통해 개발자 도구를 연다.

![image](https://user-images.githubusercontent.com/120306359/216122649-58c410e3-ad91-4b74-8655-32e7e84f520c.png)

이러한 코드를 확인할 수 있는데 여기서 2가지 사실을 알 수 있다.

날짜와 시간이 주석 처리가 되어 있다는 것과 admin.php에 접속해야 한다는 사실이다.

먼저, 웹 페이지에 admin.php를 추가하였다.

![image](https://user-images.githubusercontent.com/120306359/216123234-22fef68a-898e-49c6-81cb-3835da221096.png)

여기서도 secret password를 알지 못하기 때문에 개발자 도구를 열어 보았다.

![image](https://user-images.githubusercontent.com/120306359/216123585-0a591014-3a27-4427-9f1d-d554d69f091c.png)

유용한 정보를 얻지는 못했다.

그래서 다시 첫 번째 사실을 이용해 보았다.

![image](https://user-images.githubusercontent.com/120306359/216126995-ee6561d2-be2e-4e10-9d82-ee8d035cfed3.png)

EditThisCookie를 통해 확인해보니 쿠키가 PHPSESSID와 time까지 존재하는 것을 확인할 수 있었다.

쿠키로 time이 존재한다는 것과 앞에서 주석 처리된 날짜, 시간을 통해 time 값을 변경하는 시도를 하였다.

![image](https://user-images.githubusercontent.com/120306359/216127951-6d64d9b0-bf49-4271-90a2-a25114edd7cc.png)

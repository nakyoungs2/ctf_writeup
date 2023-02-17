해당 페이지 주소 : https://dreamhack.io/wargame/challenges/6/  

![image](https://user-images.githubusercontent.com/120306359/219546809-0028bdc6-4837-46e6-be8d-a0db5b12b08a.png)  
문제를 풀기 위해서는 페이지 접속과 파일 다운로드 2가지의 과정이 필요하다.  

![image](https://user-images.githubusercontent.com/120306359/219546945-0cdf014d-98da-46bb-9d44-9b6fbfdee906.png)  
먼저 py파일을 열면 다음과 같은 코드를 확인할 수 있다.  
users는 guest와 admin 2개라는 것을 볼 수 있다. 

![image](https://user-images.githubusercontent.com/120306359/219547130-78afac6e-03b1-41a7-a17c-7ae210df2db0.png)  
사이트에 접속을 하였다.  

![image](https://user-images.githubusercontent.com/120306359/219547183-5584a807-10b7-4f7b-824e-b53e38177c96.png)  
개발자 도구를 열어 보니 guest, guest로 로그인이 가능함을 알 수 있다. 

![image](https://user-images.githubusercontent.com/120306359/219547306-f55540f9-386b-4a6d-801f-7ec66c7ed806.png)  
로그인을 하였다. 이제 쿠키 값이 생긴 것을 확인할 수 있다.  

![image](https://user-images.githubusercontent.com/120306359/219547515-097019a7-1020-414e-9385-60644e939cca.png)  
이제 value를 admin으로 수정한 후 새로고침을 하였더니 flag 값이 나왔다.  

![image](https://user-images.githubusercontent.com/120306359/219548067-69e01c40-3e8b-4f21-b774-0e4f7558fcf2.png)  
정답은 DH{7952074b69ee388ab45432737f9b0c56}이다. 

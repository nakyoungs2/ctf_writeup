HDD를 CD-Rom으로 인식시키기 위해서는 GetDriveTypeA의 리턴값이 무엇이 되어야 하는가

![image](https://user-images.githubusercontent.com/120306359/216207589-2d4eae56-dd42-451e-b6fe-b73298704b97.png)
![image](https://user-images.githubusercontent.com/120306359/216207705-edd7e6a1-ad35-47b5-8b02-a252d3d578f1.png)

파일을 다운로드하여 실행해보면 다음과 같은 메시지를 확인할 수 있다.

UPX 패킹이 되어 있지 않음을 알 수 있다.

OllyDbg를 통해 실행을 해보았다.

여기서 GetDriveTypeA 함수를 봐야한다.

따라서 GetDriveTypeA까지 실행을 하고 그 다음 EAX 값을 보기 위해 GetDriveTypeA 다음 함수까지 BP를 걸고 실행을 한다.

EAX의 값이 00000003임을 알 수 있다.

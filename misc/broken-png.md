해당 페이지 주소 : https://dreamhack.io/wargame/challenges/104/  

![image](https://user-images.githubusercontent.com/120306359/219958576-1e76c56f-44aa-4a0a-8eeb-75848b80c33f.png)
문제 파일을 다운로드 하였다.  

![image](https://user-images.githubusercontent.com/120306359/219962050-55b1864c-1051-4ec8-beb5-d23c81188ba4.png)  
다운로드 한 파일을 열어보니 image.png 파일이 있다.  

![image](https://user-images.githubusercontent.com/120306359/219961930-91d3c6cb-90f0-4bbb-8644-9afda80517ed.png)  
깨진 이미지를 복구하기 위해 HxD Editor로 Hex code를 보았다.  
png 부분인 89 50 4E 47 0D 0A 1A 0A에는 문제가 없다.  

![image](https://user-images.githubusercontent.com/120306359/219963103-40f52603-08d0-4266-b4a0-07f114464b1b.png)  
하지만 IHDR 이후의 00 00 02 00 00 00 01 00 부분에서 문제점이 있다.  
왼쪽 4개는 이미지의 너비, 그 이후 4개는 이미지의 높이를 저장하고 있는데 문제에서 이것이 정사각형 파일이라고 하였다.  
따라서 너비와 높이를 같게 해주기 위해 02, 01 부분을 02, 02로 바꿔주었다.  

![image](https://user-images.githubusercontent.com/120306359/219963145-a0e25af5-a086-45cf-9f01-b2abee3f8c8b.png)  
이를 저장한 후에 다시 파일을 열어 보니 플래그를 확인할 수 있다.

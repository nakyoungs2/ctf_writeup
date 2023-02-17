해당 페이지 주소 : https://dreamhack.io/wargame/challenges/14/  

![image](https://user-images.githubusercontent.com/120306359/219540620-95936b8f-eb72-4080-9bd2-293106c382c5.png)  
chall0.exe 파일을 x64dbg로 열어보았다.  

![image](https://user-images.githubusercontent.com/120306359/219542855-18df7a84-c54e-43fa-8f97-149b1458782a.png)  
문자열 참조 기능을 통해 'correct'를 찾았다.  

![image](https://user-images.githubusercontent.com/120306359/219543302-ea7483f0-4553-4393-aa9c-ff02e1aa15b2.png)  
input을 받은 후에 맞으면 correct, 틀리면 wrong을 출력한다.  

![image](https://user-images.githubusercontent.com/120306359/219543395-4647b3f9-cbe1-4349-bbd9-b8b0c99235b2.png)  
쭉 함수를 따라가며 살펴보니 FLAG로 보이는 문자열을 찾을 수 있었다.  

![image](https://user-images.githubusercontent.com/120306359/219543700-206bb689-c786-4748-940a-83f571e92ab0.png)  
정답은 DH{Compar3_the_str1ng}이다.

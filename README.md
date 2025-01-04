<img width="335" alt="ImNotSpecial" src="https://github.com/user-attachments/assets/f4fc8f5b-a050-4471-8ffc-c288d3ce0f1e" />### 작동 과정
1. 맥북에서 iphone 미러링 기능을 사용해 아이폰 화면을 실시간 미러링해 맥북 화면에 접근할 수 있게 한다.
2. 스크린샷 단축키(command+shift+4)를 눌러 아이폰 화면 속 단어들이 있는 부분 사각형의 왼쪽 위, 오른쪽 아래 꼭짓점의 좌표를 구한다.
3. (x_start, y_start) 좌표에서 스크린샷을 시작하고, width, height 만큼 라이브러리를 사용하여 스크린샷을 자동으로 찍은 후, 새로운 폴더를 생성해 그 폴더 안에 스크린샷 이미지를 자동으로 저장한다.
4. 해당 스크린샷을 OCR로 이미지 분석을 하여 한글 단어를 인식하고 글자 하나 하나를 배열로 나열한다.
5. 가장 적게 나온 단어를 찾고, 그 단어가 최대 좌표가 (width, height)인 스크린샷 이미지에서 어느 좌표에 위치하고 있는지 찾고, 그 좌표의 x, y에 각각 x_start, y_start 만큼 더해서 맥북 화면에서 보여지는 정답 단어의 좌표를 구한다.
6. 자동 클릭 라이브러리를 사용해 정답 단어가 있는 좌표로 커서가 자동으로 이동하여 클릭할 수 있도록 한다.
![IMG_4529](https://github.com/user-attachments/assets/2cae473b-ea84-442c-956a-b96b29e6c46c)

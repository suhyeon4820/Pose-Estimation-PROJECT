## 회의 개요

>5월 20일 주간 회의 진행 (멀티캠퍼스 역삼)

1. 서비스 화면 100% 구현 완료 및 테스트

2. 이미지 Classification을 위한 Pose 데이터 전처리 완료

3.  향후 계획 수립

   

## 회의 내용

>주요 내용

1. 서비스 화면 100% 완료
- tkinter를 활용한 게임 위젯 화면 설계 완료

   - 기능 추가 1 : 웹캠 인식 화면과 제공되는 포즈 화면을 하나로 합침 
     - frame[ y1:y2, x1:x2 ] = img

   - 기능 추가 2 : 웹캠 인식 동작과 제공되는 포즈 class가 일치 시 매칭 화면 팝업
     - 시사점 : tkinter는 한 동작이 끝나면 자동적으로 다음 동작으로 넘어가지 못해 다양한 서비스 구현 제약 발생
   - 서비스 구현 : pyinstaller를 활용해 .py를 .exe 변환에 성공

2. Pose 이미지 데이터 전처리 - skeleton 출력
   - 검출 정확도 향상을 기존 그레이스케일 처리한 이미지를 검은색 이미지에 skeleton만 나오도록 전처리 진행

   - 배경이 사라지고 포즈의 skeleton만 출력되었기 때문에 CNN 검출 정확도 향상될 것으로 예상

     

## 결정사항

>예정 사항

1. 전처리한 데이터를 취합해 CNN 모델링 및 성능 비교할 예정
2. django활용 .exe파일을 다운로드 받을 수 있는 웹페이지 제작
3. 게임 gui디자인 진행


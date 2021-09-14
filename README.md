# YOLOv3을 이용한 영상처리 시스템 구현
운전자 및 동승자 영상 추출 skeleton 및 딥러닝을 이용한 교통사고 모니터링 시스템 개발 (딥러닝, YOLOv3)
  
- 관련 동영상  
[![Video Label](http://img.youtube.com/vi/D_dUjy80sQ4/0.jpg)](https://youtu.be/D_dUjy80sQ4?t=0s)     


## :computer: Used
- YOLOv3
- Darknet
- Head Pose Estimation
- Google Colab
- Python


## :+1: Achievement
1) 졸업 논문 제출 
2) 한국통신학회 동계 학술대회 학부부문 참여
https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE10547834
3) 한국통신학회 논문 투고 
4) 슈퍼챌린지 해커톤 참여 : 인기상 수상


## :memo: Summary

기존의 차량 긴급구난체계 서비스의 경우 사고 위치 및 발생 시각과 같은 사고에 대한 정보는 정확히 제공되지만, 환자의 상태에 대한 정보가 부족하여 정확한 응급조치를 하기 어렵다는 단점이 있다. 본 시스템은 교통사고 발생 시 블랙박스 내부 영상과 제안된 객체 인지 알고리즘을 구현한 응용시스템을 통해 사고상황을 비교적 정확히 감지하고, 실시간으로 탑승자의 부상과 관련된 정보를 제공하는 시스템을 제안한다. 본 시스템에서는 사고상황을 정확히 파악하기 위해 YOLO를 이용하여 사고의 형태를 구분한다. 사고로 판단될 경우, 머리 자세 추정 기법과 HSV(Hue Saturation Value) 컬러 모델을 이용하여 탑승자의 부상 정도와 출혈 여부 등의 상태를 파악해 관련 정보를 수집한 후, 탑승자의 휴대폰과 연동된 어플리케이션을 이용하여 긴급 구조기관에 전송한다.

| 이용 데이터 갯수              | 이미지  | 동영상 |
| :--------------------------- |:------:| -----:|
| (Leanring) normal state      | 1000   | 62    |
| (Leanring) accident state    | 1000   | 55    |
| (Test) normal state          | 855    | 29    |
| (Test) accident state        | 50     | 15    |


## :mag: Content
- 제안된 긴급구난체계 서비스 시스템 모델  
![image](https://user-images.githubusercontent.com/40004210/133212792-a7d027bc-d1ae-4432-a32f-3a50a896dd5c.png)  


- 교통사고 발생 시, 사고 감지  
![image](https://user-images.githubusercontent.com/40004210/133213065-76072736-dc40-45f6-93fd-f9aff8bfc55d.png)
![image](https://user-images.githubusercontent.com/40004210/133213077-31fb1970-57a0-4aa2-abd7-1191c6c0139e.png)  


- 교통사고 발생 시, 목 꺾임 감지   
![image](https://user-images.githubusercontent.com/40004210/133213285-3c0f0a3a-074d-4f60-95a2-d52e6c933edc.png)
![image](https://user-images.githubusercontent.com/40004210/133213290-6d9489e2-4a54-4070-967b-42ae3f08838b.png)  


- 긴급 구조기관에 전송하기 위해 데이터 수집 및 처리 시스템에 의해 처리된 데이터  
![image](https://user-images.githubusercontent.com/40004210/133213328-12210dac-530d-46d5-ad95-ea8a218fb5bc.png)  

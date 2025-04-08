# 영상내 개인정보 비식별화 서비스 개발

# Summary

<img src="images/Screenshot 2025-04-08 170910.png" width=800></br>

- 자체 데이터셋을 사용하여 영상내 얼굴, 차량 번호판 등 개인정보 인식 모델 학습 (Python, C++)
- 추론 프로세스를 Docker Image화
- AWS ECS/Batch를 활용해 API 서버 구축
- 웹 기반 사용자 UI 개발 (PHP)

# Project

## Overall Process

<img src="images/Screenshot 2025-04-08 171152.png" width=800></br>

1. 유저가 웹에서 업로드 한 영상이 S3에 저장됨
2. 트리거 된 lambda가 영상의 메타데이터 추출 후 DB에 기록
3. 유저가 영상 변환 요청 시 해당 영상 정보와 함께 Batch Task를 실행
4. 추론 프로세스를 수행하는 Docker Image가 ECS 내에서 실행
5. 작업 완료시 처리된 영상을 S3에 저장, 유저에게 완료 알림 전송

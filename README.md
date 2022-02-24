# AWS-ETL

1. Glue
ETL.py로
날짜별로 생성된 EventData / AttributionData (CSV 형식)을
1) S3 버킷 내 날짜에 맞는 폴더 생성 후, 업로드
2) GLUE Job 생성, ETL 작업 실행 
    - (Transform;Schema설정 및 Parquet 변환)
    - glue-event-job.py / glue-attribution-job.py
3) 작업 완료시 GLUE Crawler 생성, 작업 실행
    - Athena에 연결되는 데이터베이스 내 테이블


다음 작업 : EMR Cluster 생성 및 ETL 작업 실행
https://github.com/KimHyeonn/AWS-ETL-EMR

## 📂 프로젝트 구조

```plaintext
project/
│── manifests/                      # Kubernetes 배포 및 서비스 설정
│   ├── frontend-deployment.yaml   # Nginx 프론트엔드 배포
│   ├── frontend-service.yaml      # Nginx 서비스 (NodePort)
│   ├── backend-deployment.yaml    # Flask 백엔드 배포
│   ├── backend-service.yaml       # Flask 서비스 (ClusterIP)
│   ├── database-deployment.yaml   # MariaDB 배포
│   ├── database-service.yaml      # MariaDB 서비스 (ClusterIP)
│── flask-app/                     # Flask 백엔드 애플리케이션 (Dockerfile 필요)
│   ├── app.py                     # Flask 애플리케이션 코드
│   ├── requirements.txt           # Python 패키지 목록
│   ├── config.py                  # DB 연결 설정
│── nginx/                         # Nginx 설정 파일 (nginx.conf 필요)
│── db-init/                        # MariaDB 초기 설정 파일
│   ├── init.sql                    # 데이터베이스 초기화 SQL 파일

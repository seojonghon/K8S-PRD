project/
│── manifests/
│   ├── frontend-deployment.yaml   # Nginx 프론트엔드 배포
│   ├── frontend-service.yaml      # Nginx 서비스 (NodePort)
│   ├── backend-deployment.yaml    # Flask 백엔드 배포
│   ├── backend-service.yaml       # Flask 서비스 (ClusterIP)
│── flask-app/                     # Flask 백엔드 앱 (Dockerfile 필요)
│── nginx/                         # Nginx 설정 파일 (nginx.conf 필요)

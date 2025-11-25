FROM mysql:8.0

# non-root 사용자 생성
RUN groupadd -r myuser && useradd -r -g myuser myuser

# 환경 변수
ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=joondb

# 권한 제한
USER myuser

EXPOSE 3306

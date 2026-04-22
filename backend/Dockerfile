# 1. 자바 21 실행 환경 (광민님 프로젝트 설정에 맞춤)
# FROM openjdk:21-jdk-slim 대신 아래 줄로 교체
FROM eclipse-temurin:21-jdk-alpine

# 2. 빌드된 JAR 파일을 컨테이너 내부로 복사
# 반드시 ./mvnw package 명령어가 성공하여 target 폴더에 jar 파일이 있어야 합니다.
COPY target/*.jar app.jar

# 3. 컨테이너가 시작될 때 실행할 명령
ENTRYPOINT ["java", "-jar", "/app.jar"]
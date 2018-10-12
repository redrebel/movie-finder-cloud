본 프로젝트는 [movie-finder](https://github.com/heejunghwang/movie-finder)를 fork하여 cloud 버전으로 작업하였다.

movie-finder에 대한 자세한 설명은 아래를 참조한다.
# movie-finder
> 오픈소스 검색엔진인 Elasticsearch 를 활용하여 '영화'를 검색을 하는 Vue.js 프로젝트  
https://github.com/heejunghwang/movie-finder



### 1. Docker 이미지 파일 생성시
  ~~~ bash
    # vue 프로젝트를 빌드한다.
    $ npm run build
    
    # docker 이미지를 생성한다.
    $ docker build -t movie-finder .
    
    # docker 이미지를 실행(컨테이너 생성 실행)한다.
    $ docker run -d -p 8080:8080 movie-finder
    
    # 실행 중인 컨테이너의 ID 를 확인한다.
    $ docker ps 

    # 컨테이너의 log를 확인한다.
    $ docker logs -f [컨테이너 ID]
  ~~~

### 2. Kubernetes 사용시
  ~~~ bash
    # kubectl apply -f movie.yml
  ~~~


## Additional Link
* 자바카페 블로그 : http://tech.javacafe.io/
* 자바카페 git : https://github.com/JAVACAFE-STUDY

- Front-end
  - vue : 2.6.14
  - bootstrap-vue : 2.22.0
  - vue-geolocation-api : 0.1.21
  - vue-split-carousel : 1.1.1
- Back-end
  * dj-rest-auth      2.2.4
  * Django : 3.2
  * django-allauth : 0.50.0
  * django-imagekit : 4.1.0
  * django-restframework : 0.0.1
  * djangorestframework : 3.13.1

---

## 핵심 기능

* Accounts
  * 회원가입 Custom
    * 프로필 이미지
    * 좋아하는 장르 선택
  * 회원정보 수정

* 영화 정보
  * 약 10000개 의 영화 데이터
  * 약 10000개의 배우 데이터
  * 약 20개의 장르
  * axios로 상영작, 개봉작 실시간 반영
  * 검색 기능을 통한 영화 검색 가능 (띄어쓰기 무시)
  * 키워드별 영화 정렬 (역순까지)
  * 영화 디테일로 배우 정보 관람 가능
* 추천 알고리즘
  * 좋아하는 장르 기반 추천 알고리즘
* 커뮤니티
  * 각 영화 별로 댓글 작성 가능
  * 댓글을 통해 다른 유저의 프로필 관람 가능
  * 다른 유저의 추천 목록 관람 가능
* 영화관찾기
  * 위치 api와 kakao api를 이용하여 가까운 영화관 찾기



---

## installation

* back

```bash
$ pip install -r requirements.txt
```

```bash
$ python manage.py migrate
$ python manage.py loaddata movie_data.json actor_data.json genre_data.json
$ python manage.py runserver
```

​		secrets.json

```json
{
    "SECRET_KEY" : add Django Key here!
}
```

​		.env

```
TMDB_API_KEY = add TMDB API Key here!
```

---

* front

```bash
$ npm install
$ npm run server
```

​		.env.local

```
VUE_APP_TMDB_KEY = add TMDB API Key here!
VUE_APP_KAKAO_MAP = add kakao map API Key here!
```



## ERD

![image-20220601160906826](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/image-20220601160906826.png)



## 기능 구현

![image-20220601162313140](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/image-20220601162313140.png)



![image-20220601162347726](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/image-20220601162347726.png)











![1](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/1.gif)









![2](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/2.gif)









![3](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/3.gif)





![4](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/4.gif)







![2022-06-01 16;47;23](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/7.gif)















![5](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/5.gif)













![image-20220601163905548](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/image-20220601163905548.png)







![sidebar](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/map.PNG)







![6](https://github.com/ssafyFirst/.github/blob/main/profile/README.assets/6.gif)

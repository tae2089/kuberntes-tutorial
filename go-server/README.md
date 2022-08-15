## 해당 폴더는 쿠버네티스 Pod를 테스트하기 위해 만든 코드들입니다.

### 코드 설명

code는 go로 구성되어 있으며 gin-gonic 프레임워크를 사용했습니다.
또한, Dockerfile을 생성할 때에는 scrath 이미지를 활용하여 생성되었습니다.

### Dockerfile을 통해 이미지 생성하기

OS가 linux가 아니거나 arm64를 사용할 때

```shell
docker build -t <docker 계정>/이미지명:태그 --platform linux/amd64 .

ex) docker build -t tae2089/gin:1.0.1 --platform linux/amd64 .
```

OS가 linux이고 amd64를 사용할 때

```shell
docker build -t <docker 계정>/이미지명:태그 .

ex) docker build -t tae2089/gin:1.0.1 .
```

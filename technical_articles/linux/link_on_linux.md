[Up](./index.md)

# Link on Linux

리눅스에서 링크는 심볼릭링크와 하드링크 두가지가 있습니다.

심볼릭링크는 원본 파일 이름을 가리키도록 링크만 한 것으로 윈도우즈의 바로가기와 유사합니다. 심볼릭링크에서 원본 파일 이름이 존재하지 않으면 콘솔에서 블링크하여 원본 파일 이름이 없다는 것을 표현하기도 합니다. 심볼릭링크는 다른 디스크에서도 연결할 수 있습니다.

하드링크는 같은 파일에 다른 이름의 파일 이름이 존재하는 것이라고 할 수 있습니다. 서로 다른 파일 이름이기때문에 하나를 삭제하더라도 나머지 파일 이름은 남아 있기 때문에 원본 파일이 계속 존재 합니다. 하드링크는 하나의 파일을 서로 다른 파일 이름이 공유하는 것이기 떄문에 동일 디스크내에서만 생성 할 수 있습니다.

심볼릭링크 생성은 다음과 같습니다.

```sh
ln -s <원본파일경로> <대상파일경로>
```

하드링크 생성은 다음과 같습니다.

```sh
ln <원본파일경로> <대상파일경로>
```

## 참조

- [What is the difference between a hard link and a symbolic link?](https://blog.usejournal.com/what-is-the-difference-between-a-hard-link-and-a-symbolic-link-8c0493041b62)
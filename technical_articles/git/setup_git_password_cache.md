[Up](./index.md)

# git 비밀번호 캐시 설정 방법.

github나 bitbucket 같은 원격 저장소를 사용할 경우 비밀번호 입력을 요구 합니다. 때로 불편하기도 한데요. 일정 시간동안 비밀번호를 시스템에 저장하고, 비밀번호 입력을 생략할 수 있습니다. 리눅스의 경우 CLI에서 다음을 설정하면 됩니다.

```shell
git config --global credential.helper 'cache --timeout=500000'
```

이후 비밀번호를 입력하면 지정한 초단위 시간만큼 비밀번호를 캐시에 저장되며,지정한 시간동안 비밀번호를 다시 입력할 필요가 없습니다. 단, 운영체제를 다시 시작하면 이 설정은 삭제 됩니다. `.profile` 등에 설정하여 로그인시마다 설정 할 수 있습니다.


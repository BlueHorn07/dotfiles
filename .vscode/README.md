# Settings

macOS 기준, 아래 경로에 `settings.json` 파일이 있음.

```fs
~/Library/'Application Support'/Code/User
~/Library/'Application Support'/Cursor/User
```

참고로 `settings.json`은 extended JSON 포맷이기 때문에, JSON 내부에 comment 작성도 가능함.

```bash
$ jq -S . settings.json > tmp.json && mv tmp.json settings.json
```

`jq -S . settings.json > settings.json` 하게 되면, `>`의 리다이렉션이 먼저 평가 되면서, `settings.json`을 빈 파일로 초기화 해버림...;;


# Extensions

```bash
code --list-extensions
cursor --list-extensions
```

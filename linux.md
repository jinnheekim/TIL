# Linux

- mkdir(make directiry)

```
mkdir temp # temp라는 폴더 생성
mkdir -p
```

- touch
```
touch test.txt # test.txt test라는 이름으로 파일 생성
```

- echo
```
echo '안녕하세요'
```

- `>`: 새로쓰기, `>>`: 덧붙이기

```
echo 'hello' > test.txt # 새로 쓴다 (있으면 덮어쓰기)
echo 'world' >> test.txt # 끝에 덧붙이기
ls > test.txt # ls의 출력값을 test.txt에 쓰기
```

- 파일 내용 보기
    - cat: 전부 출력
    - head -3: 앞부분 출력(옵션을 입력하는 경우 그줄만큼)
    - tail: 뒷부분 출력
    - less: 새로운 레이어에 출력

- cp(copy), mv(move), rm(remove)
    -     rm -r : 폴더 삭제, 재귀 리컬시브
    
    ```
    cp test.txt temp (복사)
    mv test.txt temp2 (이동)
    mv test.txt result.txt (이름 바꾸기, 같은 폴더에서 이동)
    rm (휴지통 개념 X, 파일을 지우는게 기본값, 삭제시 주의)
    rm -r : 폴더 삭제
    ```

- grep, |

```
grep touch linux.md # linux.md에서 touch가 들어간 줄 출력

```

ls -l | grep linux # ls -l 출력결과 중에서 linux가 들어간 줄만 보기

- which 
    - 이 명령어가 어디있는지 출력
    ```
    which node(node 명령어)
    ```

- --help: 거의 대부분 명령어의 설명 출력
```
(명령어) --help
```
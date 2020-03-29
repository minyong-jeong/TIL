# Shell 명령어 실행법

Python에서 Shell 명령어를 실행하고 싶을 때가 있습니다.

파이썬의 subprocess를 활용하여 shell 명령어 실행하는 예제코드를 작성해보았습니다.

※ subprocess는 새로운 프로세스를 생성하여 input/output/error pipes와 연결을 제공하는 파이썬의 모듈

```bash
import subprocess

def run_shell_cmd(cmd):
    cmd_list = cmd.split(' ')
    try:
        sp = subprocess.run(cmd_list, stdout=subprocess.PIPE)
        print(sp.stdout.decode("utf-8"))
    except Exception as e:
        print(e)

my_cmd = 'echo test!!'
run_shell_cmd(my_cmd)
```

---
# subprocess 로 하위 프로세스 생성
```bash
cp = subporcess.run(['ls', '-l'],     #인자로 넘길 명령어
                    capture_output = True,    # stdout, stderr 캡쳐
                    universal_newlines = True,  
                    check = True)             # 오류 처리
```
                   
```
#!/user/bin/env python # 맨윗줄 추가시 python 'file_name.py' 대신 바로 'file_name.py'로 프로그램 실행 가능
```


___
# argparse 사용
```python
import argparse

parser = argparse.ArgumentParser(description='Process some integers.')      # 파서 객체 생성
parser.add_argument('integers', metavar='N', type=int, nargs='+',           # 위치 기반 명령 추가
                    help='an integer for the accumulator')                  # 도움말 추가
parser.add_argument('--sum', dest='accumulate', action='store_const',       # 옵션 인수 추가
                    const=sum, default=max,                                 
                    help='sum the integers (default: find the max)')        # 도움말 추가

args = parser.parse_args()                                                  # 파서를 이용해 인수 파싱
print(args.accumulate(args.integers))                             
```
***


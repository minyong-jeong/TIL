# 프록시 설정

SSH를 이용하여 우회하여 인터넷에 접근하는 방법을 정리하였습니다.

## putty -> ssh -> tunnels 설정

1. source port에 10000을 입력
2. dynamic을 선택
3. Local port accept connections from other hosts 체크

## Firefox 설정

1. 설정 - 연결설정
2. 수동으로 프록시 설정 선택
3. SOCKS 호스트에 localhost 포트에는 10000을 입력

# SSH 포트포워딩

1. 서버에 접속하여 8080 포트를 22 포트로 매핑

    ``` bash
    socat TCP-LISTEN:8080,fork TCP:localhost:22
    ```

    or

    ```bash
    ssh -L 0.0.0.0:8080:localhost:22 localhost
    ```

2. Remote 포트포워딩을 이용하여 PC:5000 <- server1:5000 <- server2:8888 연결

    ``` bash
    ssh -R 5000:127.0.0.1:5000 <id>@<server1-ip> -p 8080
    ssh -R 8888:127.0.0.1:5000 <id>@<server2-ip>
    ```

3. 전체 흐름

    ```bash
    # [Forward 흐름]  PC     ->  8080(->22)    ->  ssh(서버)
    # [Reverse 흐름]  5000   <-  5000          <-  8888
    ```

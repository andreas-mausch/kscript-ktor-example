- Install [kscript](https://github.com/holgerbrandl/kscript)
- Run `kscript ./ktor.kscript`
  ```
  21:33:37.830 [main] INFO ktor.application - No ktor.deployment.watch patterns specified, automatic reload is not active
  21:33:37.865 [main] INFO ktor.application - Responding at http://0.0.0.0:8080
  ```
- Test it works `curl -v http://0.0.0.0:8080`
  ```
  *   Trying 0.0.0.0...
  * TCP_NODELAY set
  * Connected to 0.0.0.0 (127.0.0.1) port 8080 (#0)
  > GET / HTTP/1.1
  > Host: 0.0.0.0:8080
  > User-Agent: curl/7.64.1
  > Accept: */*
  > 
  < HTTP/1.1 200 OK
  < Content-Length: 12
  < Content-Type: text/plain; charset=UTF-8
  < 
  * Connection #0 to host 0.0.0.0 left intact
  Hello World!* Closing connection 0
  ```

# QUICKWIT 
## Get start quickwit
https://quickwit.io/docs/get-started/quickstart
* Run quikwit via Docker:
  ```
  docker run -d -p 7280:7280 --name quickwit quickwit/quickwit:latest run
  ```
## Log collector using FluentBit
https://docs.fluentbit.io/manual/installation/docker
https://quickwit.io/docs/log-management/send-logs/using-fluentbit
* Run fluent-bit via Docker:
  ```
  docker run -p 127.0.0.1:24224:24224 -d --name fluent-bit fluent/fluent-bit:3.2.2 /fluent-bit/bin/fluent-bit -i forward -o stdout -p format=json_lines -f 1
  ```

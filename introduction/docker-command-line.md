# Docker 常用指令

## Image 相關

* search：搜尋 Image
* pull：下載 Image
* rmi：刪除不再使用的 Image

## Container 相關

* ps：查看啟動中的 Container
* run：建立一個新的並且直接啟動 Container
* create：建立一個新的 Container，必須搭配 start 才會啟動
* start：用 Conainer ID 啟動 Container
* restart：重新啟動 Container
* stop：停用 Container
* kill：強制關閉 Container
* inspect：查詢 Container 資訊
* stats：查看所有 Container 耗用資源的程度
* logs：查看 Container 的 Log
* cp：複製檔案到 Container 內的指定路徑
* rm：移除不再使用的 Container
* network：建立 docker 網路

# Remove all images and containers
```
#!/bin/bash
# Delete all containers
docker rm $(docker ps -a -q)
# Delete all images
docker rmi -f $(docker images -q)
```



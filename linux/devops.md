# 运维

## 查端口号
查看端口号被哪个进程占用：`lsof -i:9000`

## 查看内存情况
`free -m`、`free -h`、`watch -n 1 free`

## 查看进程情况
`top`， C m

## 查看文件使用
`df -h`、`du -sh /*`

## kill
发送指定的信号到相应进程。不指定型号将发送SIGTERM（15）终止指定进程。如果任无法终止该程序可用“-KILL” 参数，其发送的信号为SIGKILL(9) ，将强制结束进程，使用ps命令或者jobs 命令可以查看进程号。root用户将影响用户的进程，非root用户只能影响自己的进程。
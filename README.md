
pip install redis==2.10.6
不然redis版本太高

https://m.jd.com/ 查看key and pin



# Sign
签到啦

(目前支持京东京豆、南航、川航、携程)

运行项目

`pip install uvicorn fastapi httpx loguru diskcache apscheduler redis -i https://pypi.doubanio.com/simple/`

`uvicorn sign:app --host 0.0.0.0 --port 8081`

nohup uvicorn sign:app --host 0.0.0.0 --port 8081 > uvicorn.log &


打开 http://127.0.0.1:8081/docs

通过接口添加账户token等

apschedule调度运行,也可使用crontab运行,apschedule调度运行,也可使用crontab运行，使用apscheduler需安装redis, 使用crontab则不需要

后续增加其它平台

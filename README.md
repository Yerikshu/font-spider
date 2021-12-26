# 爬虫蛋卷基金的项目，包括了node和deno代码
- 温馨提示
  - 基金有风险，买入须谨慎
  - 爬虫的时候建议不要太频繁，把对方网站搞挂了也是有风险的
  - 可以根据自己喜好调整筛选基金条件，当然你可以设置1000%的收益率

# 配置deno环境
如果本地没有安装deno的话，而且你是在windows环境那直接用以下脚本就行了，其他环节自己找吧哈哈哈哈
```shell
iwr https://x.deno.js.cn/install.ps1 -useb | iex
```

# 运行deno的代码
- 有网络请求的：
    - deno run --allow-net denoFund.js
- 读取文件的：
    - deno run --allow-net --allow-read --allow-write denoFund.js 
- 允许所有权限
    - deno run --allow-all denoFund.js
# 运行node的代码
 - node nodeFund.js

# 运行结束之后是json文件还需要执行一下json 转excel

这个是需要的依赖
```shell
pip install tablib[all]
```

之后执行
```python
python j2excel.py
```
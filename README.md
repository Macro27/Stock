# Stock
终端实时获取股票价格

用途:
    实时查询股票价格，默认查询沪指、深指
    结果输出到终端

使用:
    例如: 查询 智慧农业 sz000816
    输入 python stock_terminal.py sz000816
    支持查询多个股票
    例如: 
    python stock_terminal.py sh601003,sz000816,sz000778,ss600221

实现:
    通过调用新浪股票API，实时查询股票价格
    支持查询多支股票，通过多线程同时查询结果
    通过Queue实现线程池

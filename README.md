# TmallSpider
![表结构](https://github.com/joson1205/TmallSpider/blob/master/table.jpg?raw=true)

## 使用
    * 如果是第一次使用,请先运行 setting.py 文件,创建相关表
    * 完善 seller 表信息,包含 shop_id,sellerNick,BC_type,url
    * 执行 detail_info.py 开始获取数据
## 说明
    可以直接录入商品id到表中,如果表中存在id字段,可以直接执行获取对应的数据,不一定需要依赖 seller 表.
    店铺有新上架商品,update_itemID.py 可直接将商品ID更新入库
## 注意
    代码采用的是基本的单线程模式,而且未使用代理,设置默认5秒一次循环;
    每小时执行一次,并未发现异常,抓取速度过快容易被限制ip,以及强制登陆;
    多次测试过,首先会要求你强制登陆,然后限制ip访问,如果没登陆的情况,不会直接限制ip



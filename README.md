# UnionPay-Geek-Challenge-数据建模赛道
rank 16th
link:https://college.upaas.unionpay.com/upgeek-web/geek/datamodeling
本次大赛基于脱敏和采样后的约 40,000 条用户消费行为数据，预测在未来的一段时间内，用户对于某产品是否会有购买和收藏的行为。  参赛团队需要设计相应的算法进行数据分析和处理，比赛结果按照指定的评价指标使用在线评测数据进行评测和排名，得分最优者获胜。(我们将考核对于在未来 7 天（即第 31 天至第 37 天）内，一名用户是否会购买和收藏一个产品的准确性。)


数据背景

本数据集为经过脱敏和采样后用户在某网站的消费行为数据，其中大致包含了三大类信息，即用户的基础信息，商品的基础信息，用户的行为信息，其中用户的基础信息除了用户的id之外皆为脱敏后的具体行为信息，商品信息除卖家id、商品id 之外皆为脱敏后的具体商品信息， 用户的行为信息包含了两个用户的具体行为（收藏和购买），除此之外都是脱敏后的具体行为信息。


日期信息进行统一编号，第一天编号为 01， 第二天为 02，以此类推。所有的特征（除上文中已经说明的之外）无具体指代。
列名 类型 说明 示例 
user_id String 用户唯一标识（脱敏后） abc123 
Product_id String 产品id（脱敏后） abc123 
seller String 卖家id（脱敏后） abc123 
day String 日期 12,..30 
action_type Int 行为相关变量（脱敏后） 1 
ProductInfo_X Int 产品相关变量 1,50,100 
Webinfo_X Int 网络行为相关变量 1,50,100 
UserInfo_X Int 用户相关变量 1,50,100 
purchase Int 用户是否购买 0,1 
favorite Int 用户是否收藏 0,1 

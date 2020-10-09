# bairong-data-mining
毕业论文进度记录
# 研究目的
## 必要性
* 互联网消费信贷自产生以来，互联网消费信贷市场规模迅猛扩张，极大地推动我国的金融行业的发展，然而，由于我国消费信贷信用风险管理滞后，导致的其违约事件爆发，鉴于互联网特性致使其风险呈几何级的放大。
	* __银行传统的信用评估：__  __缺乏收入、储蓄和消费的信息，只有还款信用的评估__，已经不适合互联网金融。
	* __互联网电商大数据信用评估：__ 基于对互联网的用户在进行网上购物、线上交易以及社交等平台的碎片化信息进行挖掘，但是 __缺乏跨平台的信息共享__。其中一些人利用不同机构提供的不同的消费类信贷产品和不同账期的额度的时间差借新债换旧债，即所谓的“共债风险”。


## 现状 
* 一般学者认为互联网消费信贷由于缺乏个人相关信息，很难将传统商业银行的信用评估体系应应用于互联网消费信贷，目前的专家学者的文献研究大多主要集中在通过定性和实证检验对现有信用评估体系的不完善和问题症结分析、建立新型信用评估体系的必要性和紧迫性分析以及在总结国内外对P2P网贷个人信用评估研宄观点和实施现状的基础上提出了对建立新的信用评估指标体系的借鉴与启示方向

# 提纲
![image](https://raw.githubusercontent.com/duanxuskt/bairong-data-mining/main/images/新评估方法.png)

### 传统商业银行信贷评估方法
#### 方法概述、发展现状
### 基于消费信贷和征信系统的风控平台概述
#### 消费信贷对传统消费信贷的影响
* 不同群体的消费行为选择
* 互联网消费金融对居民消费行为的影响
#### 大数据和我国征信业的发展 
* 回溯：中国征信体系建设的历程
* 问题：当前征信建设中的数据孤岛等问题
* 展望：可以从联邦学习等视角，分析平台的数据共享和数据安全问题
### 基于消费信贷和征信系统的风控平台构建
#### 指标体系构设计
#### 指标构建和数据处理
##### 数据探查(EDA)与预处理
##### 特征工程
##### 指标的初步筛选
##### 模型训练和优化
* 初步考虑采用XgBoost+Logistic回归的集成学习
##### 指标体系优化

# 个人研究计划
## 当前进展
### EDA数据分析阶段 （详见根目录/EDA-bairong-data.ipynb）
* 统计分析了als_1568089567.csv征信数据表的字段，部分数据缺失值比例较高，共计93259 行无重复数据，833个字段，其中缺失值达到80%以上的字段有324个
![image](https://raw.githubusercontent.com/duanxuskt/bairong-data-mining/main/images/als_缺失值.png)

* 统计分析了alm_0, alm_3, alm_6, alm_9 消费数据表的字段，alm_0为最近的贷款人消费数据，但只有88105条无重复记录，后3张表各有93259,93260,93260条无重复记录。需要以alm_0表为标准，以cum_num字段为主键进行合并，并获取以3个月为单位周期的时间序列进行统计分析。

### 文献挖掘和研究阶段
* 搜集和阅读了当前基于信贷和消费行为影响的文献
* 搜集关于联邦学习、征信平台建设等方面的文献资料

     

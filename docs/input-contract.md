# 城市更新资料契约

全部楼宇、机构、居民群体、设备、交易及事件均为本地合成，不对应新闻所涉真实主体，不声称新闻中发生这些业务问题。seed.json及各同名Parquet保留完全相同的原始值；actions.json是尚未应用的后续资料。inventory.json仅记录物理大小、摘要及行数，不是业务结论。原始量纲、空值和时区按下文解释。

energy为UTC+08小时kWh，main是结算总表，sub是子表；null非零。meter_links给半开有效区间，主表已包含当时链接分表，不重复相加。occupancy为出租m2和营业小时，weather为外温。changes给机房/设备投用和known_at，不给调整量。tariffs按自然月收energy_yuan_per_kwh和demand_yuan_per_kw，后者乘当月最大小时平均kW。contracts给适用边界、收益比例、月保底及有人时comfort温度和达标比例。split分基准拟合、独立诊断、改造期。actions为非日常机房认定的后续输入，不是分析结果。

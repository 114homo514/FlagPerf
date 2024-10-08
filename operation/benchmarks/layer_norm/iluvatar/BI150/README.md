# 参评AI芯片信息

* 厂商：ILUVATAR

* 产品名称：BI150
* 产品型号：BI150
* TDP：W

# 所用服务器配置

* 服务器数量：1


* 单服务器内使用卡数：1
* 服务器型号：
* 操作系统版本：Ubuntu 20.04.6 LTS
* 操作系统内核：linux5.4.0-148-generic
* CPU：
* docker版本：20.10.25
* 内存：
* 服务器间AI芯片直连规格及带宽：此评测项不涉及服务期间AI芯片直连

# 算子库版本
FlagGems:>联系邮箱: contact-us@iluvatar.com获取版本(FlagGems最新适配版本)

# 评测结果

## 核心评测结果

| 评测项  | correctness | TFLOPS(cpu wall clock) | TFLOPS(kernel clock) | FU(FLOPS Utilization)-cputime | FU-kerneltime |
| ---- | -------------- | -------------- | ------------ | ------ | ----- |
| flaggems | True    | 0.15TFLOPS       | 0.15TFLOPS        | 0.32% | 0.32% |
| nativetorch | True    | 0.04TFLOPS      | 0.04TFLOPS      | 0.07%      | 0.07%    |

## 其他评测结果

| 评测项  | cputime | kerneltime | cputime吞吐 | kerneltime吞吐 | 无预热时延 | 预热后时延 |
| ---- | -------------- | -------------- | ------------ | ------------ | -------------- | -------------- |
| flaggems | 3686.49us       | 3694.67us        | 271.26op/s | 270.66op/s | 23472715.3us | 4727.04us |
| nativetorch | 15895.1us       | 16053.02us        | 62.91op/s | 62.29op/s | 35230.23us | 17088.85us |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗 | 单卡最大功耗 | 单卡功耗标准差 | 单卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| nativetorch监控结果 | 2132.22W | 2166.0W | 11.94W   | /     | 128.53W       | 140.0W      | 6.41W        | 350W  |
| flaggems监控结果 | 2137.5W | 2166.0W | 16.45W   | /     | 132.5W       | 138.0W      | 4.97W        | 350W  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度 | 单卡最大显存占用 |
| ---- | --------- | -------- | ------------ | -------------- |
| nativetorch监控结果 | 99.89%    | 1.804%   | 41.25°C       | 2.936%        |
| flaggems监控结果 | 98.849%    | 1.832%   | 41.79°C       | 2.954%        |
# heroliss/GA-sort

## 项目用途

个人遗传算法学习和实验框架。GA_Core 管理种群，GA_Algorithm 提供交叉/选择，ecology 定义个体、环境、评估和突变，UI 提供排序和算式演示。

## 当前状态

- 建议分类：Python 遗传算法学习/实验框架
- 生命周期：Dormant
- 最近 push：2016-12-18T15:52:54Z
- README 扫描状态：Missing

最新 push 为 2016-12-18，长期冻结。提交记录显示 v1.0 已调试、v1.4 算式测试初步正确，但也有结果待解决的记录。

## 实际运行方式

在仓库根创建旧版 Python 虚拟环境并执行 pip install -r requirements.txt；运行 python UI/main_test.py 查看遗传交换排序示例，运行 python UI/main_calculation.py 查看算式进化示例，python UI/test_calculation.py 运行测试演示。当前代码引用 time.clock，Python 3.8+ 已移除，建议使用旧 Python 或先做兼容性修复。

## 依赖与构建线索

Python（版本未锁定，建议旧版本）；deap==1.0.2。

## 目录与证据

requirements.txt 只有 deap==1.0.2；UI 下有 main_test.py、main_calculation.py、test_calculation.py。

顶层目录/文件线索：

- `.gitignore`
- `config`
- `ecology`
- `GA_Algorithm`
- `GA_Core`
- `requirements.txt`
- `UI`

## 已知限制

- 本文档只依据 GitHub 元数据、README、构建文件、入口文件和目录证据整理，未进行完整构建或端到端运行验证。
- 不确定的运行环境、密码、服务器地址和兼容版本不在此处臆测。

## 需要确认

是否保留为遗传算法学习样例？

## 后续维护建议

1. 先确认“继续维护、完成冻结、历史保留、归档候选”中的一种状态。
2. 若继续保留，再补充一条可复现的运行验证记录和截图/输出。
3. 若确认完成或废弃，只保留简短历史说明，不需要改代码。

## 证据链接

- 仓库：[heroliss/GA-sort](https://github.com/heroliss/GA-sort)
- 默认分支：master
- 主要语言：Python
- stars / forks：0 / 0
- 扫描时间：2026-10-11T05:10:08Z
## 本地验证记录

从仓库根目录运行 `python -m UI.test_calculation` 可以执行测试示例。主程序还依赖 `deap==1.0.2`，并使用现代 Python 已移除的 `time.clock`，因此不能直接保证在 Python 3.8+ 运行。

### 模型简介
稷丰•首个开源中文多模态农业大模型是由山西农业大学研发，以[MiniCPM-Llama3-V 2.5](https://github.com/OpenBMB/MiniCPM-V)为底座，基于农业领域

基于海量有监督农业领域相关数据微调，具备广泛的农业知识和智能分析能力，该模型旨在为农业领域提供全面而高效的信息处理和决策支持。
### 说明
1. 本项目仍在不断迭代更新，考虑到农业领域覆盖广泛，且存在领域数据集资源严重匮乏的问题，我们目前仅发布了在作物学相关问答数据集上的微调模型，其他领域模型我们会在后续陆续公布；
2. 本项目所提供的数据与模型仅供科研使用，严禁用于商业用途；
### 新闻
- [**2024.06.06**] 👋 👋 👋 稷丰-v1.0版本模型发布，目前模型支持10种作物病害的多模态检测与；
### 更新计划
- [ ] 覆盖更多农业相关领域, 目前仅支持作物学领域，后续将会更新园艺学、农业资源利用、植物保护、畜牧学、兽医学、草业科学、林学以及水产等学科；
- [ ] 开源预训练数据以及指令微调数据;
- [ ] 构建农业多领域评测Benchmark;
- [ ] 发布AgriAgent技术评测报告;
### 数据集说明
* 目前支持的10种农作物类型包括：苹果/樱桃/玉米/葡萄/柑桔/桃/辣椒/马铃薯/草莓/番茄;
* 文本数据部分，我们基于GLM-3-Turbo进行文本指令集构建，图像数据来自于: [这里](https://github.com/xungeer29/AI-Challenger-Plant-Disease-Recognition);
* 指令集样例形式如下：
```python

``` 
### 部分测试结果

### 模型训练
1. 开发环境搭建
```python
conda create -n agriagent python=3.10
conda activate agrima
cd AgriAgent
pip install -r requirements.txt
```
2. 指令集构建
* 按照[此说明](https://github.com/hiyouga/LLaMA-Factory/blob/main/data/README_zh.md)进行指令集构建；
* 如需获取AgriAgent微调指令集，请发送邮件至zhiweihu@whu.edu.cn与我们联系，考虑到目前我们仍然在不断扩充指令集，最终版会在适当时候进行公开；
3. 模型微调
4. Web页面测试

### 项目参与者
本项目由山西大学开发完成

项目主要开发人员：[胡志伟](https://github.com/zhiweihu1103)

若有相关使用需求或者相关数据集提供，欢迎与我们取得联系：zhiweihu@whu.edu.cn
### 致谢
1. 本项目基于现有开源项目二次开发，在此对相关项目和研发人员表示感谢。
* [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory)
## Star History
<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=zhiweihu1103/AgriMa&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=zhiweihu1103/AgriMa&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=zhiweihu1103/AgriMa&type=Date" />
</picture>

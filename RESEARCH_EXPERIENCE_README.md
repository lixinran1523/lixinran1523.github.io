# 研究经历栏目使用说明

## 概述
我已经为您的Jekyll学术网站添加了一个新的"研究经历"栏目，用于展示您的研究项目、论文和报告。

## 新增的文件和功能

### 1. 配置文件更新
- `_config.yml`: 添加了`research_experience` collection配置
- `_data/navigation.yml`: 在导航菜单中添加了"研究经历"链接

### 2. 新增目录和文件
- `_research_experience/`: 存放研究经历条目的目录
- `_pages/research-experience.html`: 研究经历主页面
- `_includes/archive-single-research.html`: 专门用于研究经历的显示模板

### 3. 示例文件
创建了3个示例研究经历文件：
- `2024-01-01-research-project-1.md`: 机器学习在医疗诊断中的应用研究
- `2023-06-01-research-project-2.md`: 自然语言处理在智能问答系统中的应用
- `2023-03-01-research-project-3.md`: 计算机视觉在自动驾驶中的应用研究

## 如何添加新的研究经历

### 1. 创建新的研究经历文件
在`_research_experience/`目录下创建新的Markdown文件，文件名格式为：`YYYY-MM-DD-项目名称.md`

### 2. 文件头部配置
每个研究经历文件需要包含以下YAML头部信息：

```yaml
---
title: "项目标题"
collection: research_experience
category: research
permalink: /research_experience/文件名
excerpt: '项目简介'
date: YYYY-MM-DD
venue: '研究机构名称'
type: '项目类型'
duration: '项目时间范围'
supervisor: '指导老师'
paperurl: '/files/论文.pdf'
reporturl: '/files/报告.pdf'
slidesurl: '/files/幻灯片.pdf'
---
```

### 3. 文件内容
在YAML头部后添加项目的详细描述，包括：
- 研究背景和目标
- 主要贡献和创新点
- 技术栈和实现方法
- 项目成果和影响

## 支持的下载链接类型

- `paperurl`: 论文PDF文件
- `reporturl`: 研究报告PDF文件  
- `slidesurl`: 演示幻灯片PDF文件

这些链接会以按钮形式显示在研究经历条目下方，方便访问者下载相关文档。

## 自定义样式

如果需要调整研究经历页面的样式，可以：
1. 修改`_includes/archive-single-research.html`模板
2. 在`_sass/`目录下添加自定义CSS样式

## 注意事项

1. 确保PDF文件放在`files/`目录下
2. 文件名使用英文和连字符，避免中文字符
3. 日期格式使用YYYY-MM-DD
4. 每个研究经历条目都会自动生成单独的页面

现在您可以通过访问`/research-experience/`页面查看新的研究经历栏目了！

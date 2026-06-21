# 构建系统说明（本地参考，不开源）

## 快速开始

```bash
# 生成全部 9 本书
python3 build_pdf.py

# 只生成语文系列
python3 build_pdf.py 语文

# 只生成英语系列
python3 build_pdf.py 英语

# 只生成某一本
python3 build_pdf.py 语文-文言文
python3 build_pdf.py 英语-语法
```

## 可用标签

语文-文学类 / 语文-非连续性 / 语文-文言文 / 语文-积累运用 / 语文-作文
英语-听力 / 英语-语法 / 英语-阅读 / 英语-写作

## 依赖

```bash
pip3 install weasyprint markdown2
```

- Python 3.12+
- weasyprint 69.0+
- markdown2 2.5+
- macOS 自带中文字体（Songti SC）

## Markdown 写作规范

见 `build_pdf.py` 中 `LABEL_MAP` 和注释。

### 标题层级
H1 (`#`) = 章标题，H2 (`##`) = 节标题，H3 (`###`) = 小节

### 粗体标签行（自动上色）
`**定义**：` `**考查频率**：` `**满分答案**：` `**审题分析**：` `**易错提醒**：` 等

### 例题块 / 满分示例块
以 `**【例题】**` 或 `**满分示例**` 开头

### 实战演练
`### 题目一` 到 `### 题目十` 自动识别

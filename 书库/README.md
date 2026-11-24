# 书库

存放食谱/烹饪理论书的结构化章节，供「小灶」检索和引用。

## 目录约定

```
书库/<书名>/
├── manifest.json      # 源文件、页数、章节、是否 OCR
├── 00-前言.md
├── 01-第一章.md
└── ...
```

## 导入

```bash
cd /Users/tommy/Robots/cook-bot
shared/.venv/bin/python scripts/kb.py ingest "/path/to/书.pdf" --title "食物与厨艺"
shared/.venv/bin/python scripts/kb.py search "美拉德反应"
```

书还没到之前，这个目录保持为空即可。支持的格式：PDF（文字版/扫描版）、EPUB、Markdown、TXT。

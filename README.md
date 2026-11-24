# 🍳 Cookbook

菜谱与烹饪书库，由 **VideoExtract** 从视频提取，平时由飞书「烹饪助手 · 小灶」维护。

## 目录约定

- **一道菜一个文件夹**：`<菜名>/<菜名>.md`
- **Markdown 是唯一源**：`.json` 是导入快照，`.html` / `.pdf` 是派生物，手改只改 `.md`
- 修改记录写在正文末尾 `## 📝 修订`，不静默覆盖原值
- 食材用量写在「食材清单」对应食材那一行（主料/辅料/调料），不另开「精确配比」小节；整批原方和现做份量写同一行，用「·」隔开并注明口径
- `书库/`：按书拆章节的食谱/理论书，供检索引用
- `_profile/`：口味档案、反馈历史
- `_archive/`：归档菜谱，不物理删除

## 常用命令

```bash
cd /Users/tommy/Robots/cook-bot
python3 scripts/cookbook.py list
python3 scripts/cookbook.py search 牛肉
python3 scripts/cookbook.py render 白灼菜心
python3 scripts/cookbook.py deliver 白灼菜心
```

索引在 `cook-bot/state/cook.db`，可随时用 `cookbook.py index --rebuild` 重建，不进本仓库。

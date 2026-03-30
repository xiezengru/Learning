我要在现有的 FastAPI + React 项目中添加一个新功能：

**目标**：新增一个"List Notes"按钮，显示所有已保存的笔记

**后端任务**：
1. 在 `app/routers/notes.py` 中新增一个 GET endpoint `/notes`
2. 该 endpoint 查询数据库，返回所有笔记的列表
3. 返回格式：`[{"id": 1, "content": "笔记内容", "created_at": "..."}, ...]`

**前端任务**：
1. 在界面中添加一个"List Notes"按钮
2. 点击该按钮时，调用 GET `/notes` endpoint
3. 在页面下方或弹窗中显示笔记列表（显示内容和创建时间）

**参考信息**：
- 数据库模型已有 Note 表
- 现有的数据库查询方式在 `app/services/` 中

请帮我实现前后端代码，并告诉我需要修改哪些文件。
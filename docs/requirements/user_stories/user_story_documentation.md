# User Stories 管理指南

本目錄用於管理專案的所有 User Stories，遵循以下結構和規範。

## 目錄結構

```
user_stories/
├── README.md          # 本文件
├── pending/           # 待處理的 User Stories
├── in_progress/       # 進行中的 User Stories
└── completed/         # 已完成的 User Stories
```

## User Story 命名規範

所有 User Story 文件應遵循以下命名格式：
```
YYYYMMDD_story_brief_title.md
```

例如：
- `20240315_user_login_feature.md`
- `20240316_password_reset.md`

## User Story 模板

每個新的 User Story 應使用以下模板：

```markdown
# [User Story 標題]

## 基本資訊
- 建立日期：YYYY-MM-DD
- 優先級：[高/中/低]
- 狀態：[待處理/進行中/已完成]
- 預計工時：[X] 人天
- 相關聯故事：[關聯的其他 Story ID]

## 使用者故事
**身為** [角色]
**我想要** [需求]
**以便** [目的]

## 驗收標準
```gherkin
場景 1：[描述]
Given [前提條件]
When [觸發動作]
Then [預期結果]

場景 2：[描述]
...
```

## 技術細節
- 相關 API：[API 端點或服務]
- 資料需求：[資料模型或結構]
- UI/UX 需求：[介面要求]
- 安全考量：[安全要求]

## 相依性
- [列出相依的系統或功能]

## 備註
- [其他相關資訊]

## 變更歷史
| 日期 | 變更者 | 變更內容 |
|------|--------|----------|
| YYYY-MM-DD | [名稱] | [描述] |
```

## 工作流程

1. **新增 Story**
   - 在 `pending/` 目錄建立新文件
   - 使用上述模板
   - 更新 `backlog.md`

2. **開始處理**
   - 將文件移至 `in_progress/`
   - 更新 Story 狀態
   - 更新 `backlog.md`

3. **完成 Story**
   - 將文件移至 `completed/`
   - 更新完成時間和狀態
   - 更新 `backlog.md`

## 注意事項

1. 確保每個 Story 都有唯一的識別碼
2. 保持文件格式一致性
3. 及時更新 Story 狀態
4. 定期清理和歸檔已完成的 Stories
5. 維護好相關文件的連結關係 
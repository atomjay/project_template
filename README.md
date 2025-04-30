# Project Template System

這是一個通用的專案模板系統，基於 Google 開發最佳實踐設計，支援 Python、Rust 和 Next.js 等多種開發環境，用於快速建立和管理新專案。

## 特色

- 📁 完整的專案結構和文檔模板
- 🔧 支援多種開發環境（Python、Rust、Next.js）
- 📝 完整的文檔管理系統
- 🚀 快速開發流程指南
- 🔍 品質保證和測試框架
- 🛡️ 安全性最佳實踐

## 目錄結構

```
project_root/
├── docs/                    # 文檔目錄
│   ├── requirements/        # 需求文檔
│   │   ├── project_requirements.md
│   │   ├── user_stories/   # 使用者故事
│   │   └── backlog.md      # 待辦事項
│   ├── design/             # 設計文檔
│   ├── architecture/       # 架構文檔
│   ├── api/               # API 文檔
│   └── development.md     # 開發指南
├── src/                   # 源代碼目錄
├── tests/                # 測試目錄
├── config/               # 配置文件
├── deployments/          # 部署相關
└── scripts/             # 工具腳本
```

## 快速開始

1. **複製模板**
```bash
git clone https://github.com/atomjay/projcet_template.git
cd project_template
```

2. **選擇開發環境**

根據你的專案需求，選擇對應的開發環境：

### Python 專案
```bash
# 方法 1: 使用 venv
python -m venv venv
source venv/bin/activate  # Linux/Mac
# 或
.\venv\Scripts\activate  # Windows

# 安裝依賴
pip install -r requirements.txt
```

```bash
# 方法 2: 使用 Conda
# 創建新的 Conda 環境
conda create -n project_env python=3.x
conda activate project_env

# 安裝依賴
conda install --file requirements.txt
# 或
pip install -r requirements.txt

# 將環境導出（可選）
conda env export > environment.yml
```

### Rust 專案
```bash
# 確認 Cargo.toml 存在
cargo build
```

### Next.js 專案
```bash
# 安裝依賴
npm install
# 或
yarn install
# 或
pnpm install
```

## 開發工作流程

1. **初始化專案**
   - 修改 README.md
   - 更新專案配置
   - 選擇開發環境

2. **開發流程**
   - 建立功能分支 (`git checkout -b feature/your-feature`)
   - 實作功能
   - 提交變更 (`git commit -m "feat: add new feature"`)
   - 發起合併請求

3. **提交規範**
   使用 Conventional Commits 規範：
   - `feat`: 新功能
   - `fix`: 錯誤修復
   - `docs`: 文檔更新
   - `style`: 程式碼格式
   - `refactor`: 重構
   - `test`: 測試相關
   - `chore`: 維護任務

## 文檔指南

所有文檔都使用 Markdown 格式，位於 `docs/` 目錄下：

- `requirements/`: 需求文檔
- `design/`: 設計文檔
- `architecture/`: 架構文檔
- `api/`: API 文檔



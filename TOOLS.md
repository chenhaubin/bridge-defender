# TOOLS.md - Local Notes

## API Keys

- Brave Search: BSAq--RwYZsQOIG24KdLylvzP0FGt9e

## Cameras

- (None configured yet)

## SSH

- (None configured yet)

## TTS

- **Provider:** Microsoft Edge TTS (edge-tts)
- **Path:** `/tmp/tts_env/bin/edge-tts`
- **Voice:** `zh-CN-XiaoxiaoNeural` (中文女声)
- **Install:** 
  ```bash
  python3 -m venv /tmp/tts_env
  source /tmp/tts_env/bin/activate
  pip install edge-tts
  ```
- **Usage:**
  ```bash
  edge-tts -t "要转换的文字" --voice zh-CN-XiaoxiaoNeural --write-media output.mp3
  ```

## Feishu Voice Messages

- **API:** `POST https://open.feishu.cn/open-apis/im/v1/files`
- **Then:** `POST https://open.feishu.cn/open-apis/im/v1/messages`
- **msg_type:** `audio`
- **Content format:** `{"file_key": "xxx", "duration": 4000}`
- **Note:** Content must be JSON string, not object

## Avatar

- **Path:** `/home/chinaman/.openclaw/workspace/avatars/claw.png`
- **Generated:** 2026-02-08 with Gemini 3 Pro Image

## GitHub 配置

- **用户名:** chenhaubin
- **Token:** (已暴露，请立即删除并重新生成)

### Git 提交规范 (Conventional Commits)

每次开发完成后必须：
1. 创建高质量 README（徽章、截图、功能列表、技术栈）
2. 遵循规范提交信息格式

```
<type>(<scope>): <subject>

[可选的详细描述]

[可选的Footer]
```

**Type 类型:**
- `feat` - 新功能
- `fix` - 修复Bug
- `docs` - 文档更新
- `style` - 代码格式（不影响功能）
- `refactor` - 重构
- `perf` - 性能优化
- `test` - 测试
- `chore` - 构建/工具变动

**示例:**
```
feat: 添加敌人生成系统

- 实现三种敌人类型
- 添加波次难度递增
- 包含粒子爆炸特效
```

### 提交工作流程

```bash
# 开发完成后
git add .
git commit -m "type: 简要描述

- 详细变更1
- 详细变更2"
git push origin master
```

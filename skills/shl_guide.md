# 环境准备
1. Install opencode: https://opencode.ai/docs

2. Install superpowers: https://github.com/obra/superpowers/tree/main (Need to re-launch opencode)

3. Copy shl folder to `~/.agents/skills/`，final path is `~/.agents/skills/shl`

# 工作流
1. SHL 右上角选 Python 3.7（这很重要！）
2. 整理题目: 拍照，OCR 提取出文字，整理好 markdown 文件
3. 进入工作目录，执行 opencode，输入“帮我完成这道 SHL 算法题 @题目文件"
4. 把当前目录中的 solution.py 文件内容手打到 SHL 上

# 技巧心得
- 可以开两个 opencode 分别给两个题目
- 有时候题1是 hard，题2反而是 easy

# opencode 常用命令
- /connect：连接哪个大模型平台的订阅服务
- /models: 切换模型
- /skills：查看支持哪些 agent skill

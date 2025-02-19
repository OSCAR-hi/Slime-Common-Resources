# Slime-New-
Reconstructed development pattern of the Slime project

## 开发注意事项

### 1. 子模块改动
- 在开发过程中，自己负责的子模块新增内容，请全部放到自己负责的子模块文件夹当中。

---

### 2. 主模块更新
- 当主模块有新内容更新，奥斯卡会告知大家。
- 随后请大家记得切换到自己Fork的主库（`Common Resources`）当中，拉取（pull）最新的代码内容。
- 如果不能成功拉取，先尝试使用`stash`指令藏匿本地主库代码的改动（local changes），再尝试拉取。
- 如若还不能正常拉取，请联系奥斯卡协助解决问题。

### 3. 主模块改动
- 如果有需要提交主模块的改动，请事先告知奥斯卡！
- 经双方确认改动是否合理后，再到Github的主库上提交pull request。

---

### 4. 提交信息规范

请遵循以下格式要求来编写提交信息：

- 以允许的小写前缀开头（如 `feat`、`fix`、`chore` 等）
- 前缀后必须紧跟冒号和空格（例如：`feat: `）
- 前缀前不可有其他字符

#### 有效示例：

- `feat: 新增尖刺方块实现`
- `fix: 修复碰撞体检测判定`

---

### 项目库中已集成了提交信息规范辅助工具，具体操作步骤如下：

##### 1. **安装 Node 版本管理器（NVM）**  
   请先下载并安装 [nvm](https://github.com/coreybutler/nvm-windows#readme)。

##### 2. **安装所需版本的Node.js**  
   执行以下命令18.0版本的Node.js：
   ```bash
   nvm install 18.0
   ```

###### 3. **安装项目依赖**  
   在主库中执行以下命令安装项目的npm依赖：
   ```bash
   npm install
   ```

###### 4. **安装Husky库**  
   随后请在每个子库的git bash中使用以下命令来手动安装Husky：
   ```bash
   npx husky install
   ```
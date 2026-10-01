# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-10-01 18:16`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 113228 | cve | 64366 | medium | 45555 |
| 2 | wordpress | 106639 | other | 58985 | low | 40028 |
| 3 | wp-plugin | 98152 | wordpress | 6353 | high | 30252 |
| 4 | low | 37858 | auth | 5018 | info | 27549 |
| 5 | medium | 36371 | sql | 4405 | critical | 17501 |
| 6 | candidate | 35208 | detect | 2711 | unknown | 143 |
| 7 | high | 18833 | microsoft | 2498 | informative | 16 |
| 8 | tech | 17736 | remote_code_execution | 2363 | meduim | 16 |
| 9 | production | 17603 | web | 1437 | hight | 15 |
| 10 | detect | 16969 | social | 1309 | cretical | 4 |

**81 个目录，44572 个文件**
## 如何使用

### 克隆项目

克隆这个项目到本地：

```bash
git clone https://github.com/lianqingsec/NucleiPocGather.git
```

进入项目目录：

```bash
cd NucleiPocGather
```

### 配置

在 `repo.txt` 文件中配置监控 GitHub 项目信息。

### 运行脚本

运行 Python 脚本：

```bash
python NucleiPocGather.py
```

### GitHub Action

在 GitHub 仓库中设置 Action，以便每日自动运行脚本。

> 需要配置`Workflow permissions`为`Read and write`权限

## 文件结构

- `NucleiPocGather.py`: 收集全网 Nuclei POC 的脚本文件。
- `DeWeight.py`: 对现有的 Nuclei POC 进行进一步去重的脚本文件。
- `WirteREADME.py`: 统计现有的 POC 并更新 README.md 文件。
- `repo.txt`: Nuclei POC 仓库列表。
- `poc.txt`: 已存档 POC 列表。
- `poc/`: 存放分类后的 Nuclei POC 文件夹。


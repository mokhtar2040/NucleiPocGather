# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-10-06 18:25`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 113224 | cve | 64357 | medium | 45497 |
| 2 | wordpress | 106616 | other | 59025 | low | 40007 |
| 3 | wp-plugin | 98130 | wordpress | 6365 | high | 30268 |
| 4 | low | 37848 | auth | 4924 | info | 27433 |
| 5 | medium | 36330 | sql | 4409 | critical | 17487 |
| 6 | candidate | 35293 | detect | 2696 | unknown | 144 |
| 7 | high | 18870 | microsoft | 2498 | informative | 16 |
| 8 | tech | 17731 | remote_code_execution | 2356 | meduim | 16 |
| 9 | production | 17502 | web | 1435 | hight | 15 |
| 10 | detect | 16886 | social | 1305 | cretical | 4 |

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


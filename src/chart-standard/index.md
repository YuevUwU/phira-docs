# Phira 谱面标准

## 谱面基本结构

Phira 谱面包是一个压缩包, 解压后的压缩包内应当直接包含以下文件而非文件夹:

- `info.yml`: 采用 YAML 格式的[谱面信息](./chartinfo.md)文件
- ...`info.yml` 中所指定的其他文件

## 各文件支持情况

### 谱面文件

见 [谱面文件格式](./chart-format/index.md)

### 音乐文件

见 [音乐文件格式](./music.md)

TBD

## 常见问题

RPE 的谱面 JSON 文件存储了元数据(创作者, 难度, 名称等), 这一行为是**不被推荐**的, 这会导致这部分信息可能被重复记录, 从而导致不一致性. Phira 的行为以 `info.yml` 为准

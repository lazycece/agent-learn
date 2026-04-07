---
name: roll-dice
description: 使用随机数生成器掷骰子。当被要求掷一个骰子（d6, d20 等）、掷多个骰子或生成随机骰子点数时使用。
---

要掷一个骰子，请使用以下命令，该命令可生成 1 到指定面数之间的随机数：

```bash
echo $((RANDOM % <sides> + 1))
```

```powershell
Get-Random -Minimum 1 -Maximum (<sides> + 1)
```

将 `<sides>` 替换为骰子的面数（例如，标准骰子为 6，d20 为 20）。
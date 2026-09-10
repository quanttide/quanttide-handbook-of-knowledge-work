# 工作区

## 目标

工作区是第二大脑的边界单位：一个领域或一个法人主体即一个工作区，以章程的二十格资产为骨架，区间彼此隔绝。

## 一般格式

```text
{domain}/
├── data/                       陈述型九宫格与不占格资产
│   ├── report/ library/ history/      过去：报告、参考、历史
│   ├── journal/ profile/ brochure/    现在：日志、档案、宣传册
│   ├── roadmap/ insight/ intention/   未来：路线图、洞察、意图
│   └── context/ archive/              默认入口与备份出口
├── docs/                       程序型的文档类
│   ├── bylaw/ specification/          宪法：章程、规格
│   ├── handbook/ gallery/             法律：手册、案例
│   └── tutorial/ essay/               法理：教程、札记
├── packages/{domain}-toolkit/  Toolkit：工具箱
├── apps/{app}/                 Platform：平台
└── examples/default/           Example：实验室
```

目录名与章程的资产类型一一对应，各资产独立成仓、父仓库只追踪引用。Context 是默认入口，Archive 是过时资产的出口；产出按流动规则转出到目标领域的对应资产，不在上游留副本。

## 流程

1. 划界：新建领域或主体即成立工作区，二十格资产按章程落位，形态如一般格式。
2. 域内流动：工作区内的资产之间按[产物规范](../artifacts/index.md)流动。
3. 跨区流动：归属判定先于搬运，步骤见[从主体到领域](../../gallery/workflows/from-default-to-domain.md)；只在自己的工作区提交，不改别区内容。
4. 登记：新工作区登记到[领域第二大脑目录](../../gallery/workspaces/domain-second-brain.md)。

## 验收

- 资产齐备：二十格按章程落位（data/ 十一件、docs/ 六件，另有工具箱、平台、实验室），Context 入口与 Archive 出口都在，对账通过。
- 每件资产是独立仓库，父仓库只追踪引用，不直接改子仓库文件。
- 与已建成的工作区并排比对结构一致——跨领域因此可关联分析。
- 区间隔绝：本区的提交不含对他区内容的直接修改。
- 跨区迁移满足流程案例的验收。
- 新工作区已登记到目录。

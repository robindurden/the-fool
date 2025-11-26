# Markdown Extension Examples

This page demonstrates some of the built-in markdown extensions provided by VitePress.

## Syntax Highlighting

VitePress provides Syntax Highlighting powered by [Shiki](https://github.com/shikijs/shiki), with additional features like line-highlighting:

**Input**

````md
the-fool/
├── LICENSE               # 版权声明（All Rights Reserved）
├── README.md             # 项目简介（极简 + 方向 + 目标）
│
├── 0-logic/              # 从0和1开始
│   ├── 01_truth-table.md
│   ├── 02_and-or-not.md
│   ├── 03_xor-nand.md
│   └── 04_boolean-algebra.md
│
├── 1-gates/              # 逻辑门 → 电路 → 加法
│   ├── 01_half-adder.md
│   ├── 02_full-adder.md
│   └── 03_multi-bit-adder.md
│
├── 2-cpu/                # 半加器 → 全加器 → CPU原型
│   ├── 01_registers.md
│   ├── 02_pc-and-instruction.md
│   ├── 03_minimal-cpu-go.md
│   └── 04_program-is-data.md
│
├── 3-math/               # 离散数学与形式基础
│   ├── 01_set-and-function.md
│   ├── 02_propositional-logic.md
│   ├── 03_induction-proof.md
│   └── 04_reasoning-as-program.md
│
└── 4-systems/            # 未来延展区（暂留）
    ├── 01_memory-model.md
    ├── 02_syscall-bridge.md
    └── 03_process-and-scheduling.md
````

**Output**

```js{4}
export default {
  data () {
    return {
      msg: 'Highlighted!'
    }
  }
}
```

## Custom Containers

**Input**

```md
::: info
This is an info box.
:::

::: tip
This is a tip.
:::

::: warning
This is a warning.
:::

::: danger
This is a dangerous warning.
:::

::: details
This is a details block.
:::
```

**Output**

::: info
This is an info box.
:::

::: tip
This is a tip.
:::

::: warning
This is a warning.
:::

::: danger
This is a dangerous warning.
:::

::: details
This is a details block.
:::

## More

Check out the documentation for the [full list of markdown extensions](https://vitepress.dev/guide/markdown).

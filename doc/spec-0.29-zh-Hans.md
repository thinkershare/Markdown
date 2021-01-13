# 核心规范

## 基础概念

### 字符集和行

1. 字符

    1. 规定字符中的字符就是Unicode代码点(code point)
    2. 不规定字符存储的编码格式,不处理字节,而是处理代码点

2. 换行

    1. line: 任意多个(包括0)非(U+000A|U+000D)字符构成的序列,以'line ending'结尾
    2. line ending: U+000A(\n), U+000D(\r), U+000DU+000A(\r\n), \r\n优先级高于\r
    3. blank line: 行由0个字符序列构成,或者只存在U+0020(空格),U+0009(制表符)字符

3. 字符类

    1. 空格(space): U+0020
    2. 空白字符(whitespace character): U+0020(space), U+0009(tab), U+000A(newline), U+000B(line tabulation), U+000C(form feed), U+000D(carriage return)
    3. Unicode空白字符: Unicode Zs, U+0009, U+000D, U+000A, U+000C
    4. 非空白字符(none-whitespace character): 除开空白字符以为的任何字符
    5. ASCII标点符号(ASCII punctuation character): `!`, `"`, `#`, `$`, `%`, `&`,
        `'`, `(`, `)`, `*`, `+`, `,`, `-`, `.`, `/` (U+0021–2F),  `:`, `;`, `<`, `=`, `>`, `?`,
        `@` (U+003A–0040), `[`, `\`, `]`, `^`, `_`, `` ` ``, (U+005B–0060), `{`, `|`, `}`, or `~` (U+007B–007E)
    6. 标点符号(punctuation character): Unicode Pc, Pd, Pe, Pf, Pi, Po, Ps

### 制表符(Tabs)

### 不安全字符

## 元素类型

## 叶块

## 容器块

## 行元素

## 补充说明

### 附加网址

-   [官网地址](https://commonmark.org)
-   [规范地址](https://spec.commonmark.org/)
-   [文档地址](https://spec.commonmark.org/0.29/)
-   [仓库地址](https://github.com/commonmark/commonmark-spec)

### 源文档

-   version: 0.29
-   date: 2019-04-06
-   author: John MacFarlane
-   license: [CC-BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

# Usage

### Adding to model
**For ease of use, simply copy the phoneme and grapheme entries with other dictionaries for the OpenUtau phonemizer to use**

### OU compatibility
To make the phoneme set compatible with [OpenUtau](https://github.com/stakira/OpenUtau), the dictionary is named "dsdict-zh.yaml", but the language tag is set to `cn/` instead of `zh/` to differenciate it from OpenCPop's phoneme system, which allows one to train with both phoneme systems without any issues.

**Below is a table for merging phonemes in the training config, `zh/` is for OpenCPop, `cn/` is for AV**
```
zh/a, cn/a
zh/b, cn/b
zh/c, cn/c
zh/ch, cn/ch
zh/d, cn/d
zh/e, cn/e
zh/E, cn/E
zh/er, cn/er
zh/f, cn/f
zh/g, cn/g
zh/h, cn/h
zh/i, cn/i
zh/i0, cn/i0
zh/ir, cn/ih
zh/j, cn/j
zh/k, cn/k
zh/l, cn/l
zh/m, cn/m
zh/n, cn/n
zh/o, cn/o
zh/p, cn/p
zh/q, cn/q
zh/r, cn/r
zh/s, cn/s
zh/sh, cn/sh
zh/t, cn/t
zh/u, cn/u
zh/uo, cn/uo
zh/ve, cn/ve
zh/w, cn/w
zh/x, cn/x
zh/y, cn/y
zh/v, cn/yu
zh/ve, cn/yE
zh/z, cn/z
zh/zh, cn/zh
```

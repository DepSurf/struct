# Struct: <code>regmap_mmio_context</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int reg_bytes;
    unsigned int val_bytes;
    unsigned int pad_bytes;
    struct clk *clk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool relaxed_mmio;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool relaxed_mmio;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool relaxed_mmio;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool relaxed_mmio;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool big_endian;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool big_endian;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool big_endian;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct regmap_mmio_context {
    void *regs;
    unsigned int val_bytes;
    bool attached_clk;
    struct clk *clk;
    void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int);
    unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*reg_write)(struct regmap_mmio_context *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*reg_read)(struct regmap_mmio_context *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int reg_bytes</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int pad_bytes</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool attached_clk</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool relaxed_mmio</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool big_endian</code>
</li>
<li>
<b>Field removed. </b>
<code>bool relaxed_mmio</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct clk *clk</code> ➡️ <code>struct clk *clk</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

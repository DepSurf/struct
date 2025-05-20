# Struct: <code>nand_ecc_ctrl</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nand_ecc_ctrl {
    nand_ecc_modes_t mode;
    enum nand_ecc_algo algo;
    int steps;
    int size;
    int bytes;
    int total;
    int strength;
    int prepad;
    int postpad;
    unsigned int options;
    void *priv;
    u8 *calc_buf;
    u8 *code_buf;
    void (*hwctl)(struct nand_chip *, int);
    int (*calculate)(struct nand_chip *, const uint8_t *, uint8_t *);
    int (*correct)(struct nand_chip *, uint8_t *, uint8_t *, uint8_t *);
    int (*read_page_raw)(struct nand_chip *, uint8_t *, int, int);
    int (*write_page_raw)(struct nand_chip *, const uint8_t *, int, int);
    int (*read_page)(struct nand_chip *, uint8_t *, int, int);
    int (*read_subpage)(struct nand_chip *, uint32_t, uint32_t, uint8_t *, int);
    int (*write_subpage)(struct nand_chip *, uint32_t, uint32_t, const uint8_t *, int, int);
    int (*write_page)(struct nand_chip *, const uint8_t *, int, int);
    int (*write_oob_raw)(struct nand_chip *, int);
    int (*read_oob_raw)(struct nand_chip *, int);
    int (*read_oob)(struct nand_chip *, int);
    int (*write_oob)(struct nand_chip *, int);
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>

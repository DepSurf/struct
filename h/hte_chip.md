# Struct: <code>hte_chip</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hte_chip {
    const char *name;
    struct device *dev;
    const struct hte_ops *ops;
    u32 nlines;
    int (*xlate_of)(struct hte_chip *, const struct of_phandle_args *, struct hte_ts_desc *, u32 *);
    int (*xlate_plat)(struct hte_chip *, struct hte_ts_desc *, u32 *);
    bool (*match_from_linedata)(const struct hte_chip *, const struct hte_ts_desc *);
    u8 of_hte_n_cells;
    struct hte_device *gdev;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hte_chip {
    const char *name;
    struct device *dev;
    const struct hte_ops *ops;
    u32 nlines;
    int (*xlate_of)(struct hte_chip *, const struct of_phandle_args *, struct hte_ts_desc *, u32 *);
    int (*xlate_plat)(struct hte_chip *, struct hte_ts_desc *, u32 *);
    bool (*match_from_linedata)(const struct hte_chip *, const struct hte_ts_desc *);
    u8 of_hte_n_cells;
    struct hte_device *gdev;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hte_chip {
    const char *name;
    struct device *dev;
    const struct hte_ops *ops;
    u32 nlines;
    int (*xlate_of)(struct hte_chip *, const struct of_phandle_args *, struct hte_ts_desc *, u32 *);
    int (*xlate_plat)(struct hte_chip *, struct hte_ts_desc *, u32 *);
    bool (*match_from_linedata)(const struct hte_chip *, const struct hte_ts_desc *);
    u8 of_hte_n_cells;
    struct hte_device *gdev;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hte_chip {
    const char *name;
    struct device *dev;
    const struct hte_ops *ops;
    u32 nlines;
    int (*xlate_of)(struct hte_chip *, const struct of_phandle_args *, struct hte_ts_desc *, u32 *);
    int (*xlate_plat)(struct hte_chip *, struct hte_ts_desc *, u32 *);
    bool (*match_from_linedata)(const struct hte_chip *, const struct hte_ts_desc *);
    u8 of_hte_n_cells;
    struct hte_device *gdev;
    void *data;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
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
<b>Regular</b>
<ul>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

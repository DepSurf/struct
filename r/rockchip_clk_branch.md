# Struct: <code>rockchip_clk_branch</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct rockchip_clk_branch {
    unsigned int id;
    enum rockchip_clk_branch_type branch_type;
    const char *name;
    const const char * *parent_names;
    u8 num_parents;
    long unsigned int flags;
    int muxdiv_offset;
    u8 mux_shift;
    u8 mux_width;
    u8 mux_flags;
    int div_offset;
    u8 div_shift;
    u8 div_width;
    u8 div_flags;
    struct clk_div_table *div_table;
    int gate_offset;
    u8 gate_shift;
    u8 gate_flags;
    struct rockchip_clk_branch *child;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rockchip_clk_branch {
    unsigned int id;
    enum rockchip_clk_branch_type branch_type;
    const char *name;
    const const char * *parent_names;
    u8 num_parents;
    long unsigned int flags;
    int muxdiv_offset;
    u8 mux_shift;
    u8 mux_width;
    u8 mux_flags;
    int div_offset;
    u8 div_shift;
    u8 div_width;
    u8 div_flags;
    struct clk_div_table *div_table;
    int gate_offset;
    u8 gate_shift;
    u8 gate_flags;
    struct rockchip_clk_branch *child;
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

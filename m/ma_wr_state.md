# Struct: <code>ma_wr_state</code>

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
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ma_wr_state {
    struct ma_state *mas;
    struct maple_node *node;
    long unsigned int r_min;
    long unsigned int r_max;
    enum maple_type type;
    unsigned char offset_end;
    unsigned char node_end;
    long unsigned int *pivots;
    long unsigned int end_piv;
    void **slots;
    void *entry;
    void *content;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ma_wr_state {
    struct ma_state *mas;
    struct maple_node *node;
    long unsigned int r_min;
    long unsigned int r_max;
    enum maple_type type;
    unsigned char offset_end;
    unsigned char node_end;
    long unsigned int *pivots;
    long unsigned int end_piv;
    void **slots;
    void *entry;
    void *content;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ma_wr_state {
    struct ma_state *mas;
    struct maple_node *node;
    long unsigned int r_min;
    long unsigned int r_max;
    enum maple_type type;
    unsigned char offset_end;
    long unsigned int *pivots;
    long unsigned int end_piv;
    void **slots;
    void *entry;
    void *content;
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned char node_end</code>
</li>
</ul>
</details>
</li>
</ul>

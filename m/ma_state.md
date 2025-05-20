# Struct: <code>ma_state</code>

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
struct ma_state {
    struct maple_tree *tree;
    long unsigned int index;
    long unsigned int last;
    struct maple_enode *node;
    long unsigned int min;
    long unsigned int max;
    struct maple_alloc *alloc;
    unsigned char depth;
    unsigned char offset;
    unsigned char mas_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ma_state {
    struct maple_tree *tree;
    long unsigned int index;
    long unsigned int last;
    struct maple_enode *node;
    long unsigned int min;
    long unsigned int max;
    struct maple_alloc *alloc;
    unsigned char depth;
    unsigned char offset;
    unsigned char mas_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ma_state {
    struct maple_tree *tree;
    long unsigned int index;
    long unsigned int last;
    struct maple_enode *node;
    long unsigned int min;
    long unsigned int max;
    struct maple_alloc *alloc;
    enum maple_status status;
    unsigned char depth;
    unsigned char offset;
    unsigned char mas_flags;
    unsigned char end;
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
<b>Field added. </b>
<code>enum maple_status status</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char end</code>
</li>
</ul>
</details>
</li>
</ul>

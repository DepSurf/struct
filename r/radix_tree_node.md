# Struct: <code>radix_tree_node</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct radix_tree_node {
    unsigned int path;
    unsigned int count;
    struct radix_tree_node *parent;
    void *private_data;
    struct callback_head callback_head;
    struct list_head private_list;
    void * slots[64];
    long unsigned int tags[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct radix_tree_node {
    unsigned char shift;
    unsigned char offset;
    unsigned int count;
    struct radix_tree_node *parent;
    void *private_data;
    struct callback_head callback_head;
    struct list_head private_list;
    void * slots[64];
    long unsigned int tags[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct radix_tree_node {
    unsigned char shift;
    unsigned char offset;
    unsigned char count;
    unsigned char exceptional;
    struct radix_tree_node *parent;
    void *private_data;
    struct list_head private_list;
    struct callback_head callback_head;
    void * slots[64];
    long unsigned int tags[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct radix_tree_node {
    unsigned char shift;
    unsigned char offset;
    unsigned char count;
    unsigned char exceptional;
    struct radix_tree_node *parent;
    struct radix_tree_root *root;
    struct list_head private_list;
    struct callback_head callback_head;
    void * slots[64];
    long unsigned int tags[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct radix_tree_node {
    unsigned char shift;
    unsigned char offset;
    unsigned char count;
    unsigned char exceptional;
    struct radix_tree_node *parent;
    struct radix_tree_root *root;
    struct list_head private_list;
    struct callback_head callback_head;
    void * slots[64];
    long unsigned int tags[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct radix_tree_node {
    unsigned char shift;
    unsigned char offset;
    unsigned char count;
    unsigned char exceptional;
    struct radix_tree_node *parent;
    struct radix_tree_root *root;
    struct list_head private_list;
    struct callback_head callback_head;
    void * slots[64];
    long unsigned int tags[3];
};
```
</details>
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
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char shift</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char offset</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int path</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char exceptional</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int count</code> ➡️ <code>unsigned char count</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct radix_tree_root *root</code>
</li>
<li>
<b>Field removed. </b>
<code>void *private_data</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
</ul>

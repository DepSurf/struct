# Struct: <code>icc_provider</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct icc_provider {
    struct list_head provider_list;
    struct list_head nodes;
    int (*set)(struct icc_node *, struct icc_node *);
    int (*aggregate)(struct icc_node *, u32, u32, u32, u32 *, u32 *);
    void (*pre_aggregate)(struct icc_node *);
    int (*get_bw)(struct icc_node *, u32 *, u32 *);
    struct icc_node * (*xlate)(struct of_phandle_args *, void *);
    struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *);
    struct device *dev;
    int users;
    bool inter_set;
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_bw)(struct icc_node *, u32 *, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct icc_node_data * (*xlate_extended)(struct of_phandle_args *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool inter_set</code>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

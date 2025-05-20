# Struct: <code>node</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct node {
    struct list_head list;
    struct audit_tree *owner;
    unsigned int index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct node {
    struct list_head list;
    struct audit_tree *owner;
    unsigned int index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct node {
    struct list_head list;
    struct audit_tree *owner;
    unsigned int index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct node {
    struct list_head list;
    struct audit_tree *owner;
    unsigned int index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct node {
    struct list_head list;
    struct audit_tree *owner;
    unsigned int index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct list_head cache_attrs;
    struct device *cache_dev;
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
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
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
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct node {
    struct device dev;
    struct list_head access_list;
    struct work_struct node_work;
    struct list_head cache_attrs;
    struct device *cache_dev;
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
<code>struct device dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct node_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct audit_tree *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int index</code>
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head access_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *cache_dev</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field added. </b>
<code>struct audit_tree *owner</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int index</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head access_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct node_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *cache_dev</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head access_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct node_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *cache_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct audit_tree *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int index</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct work_struct node_work</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct work_struct node_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *cache_dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *cache_dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct work_struct node_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *cache_dev</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>generic</code> and <code>gcp</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head cache_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *cache_dev</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

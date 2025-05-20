# Struct: <code>dev_dax</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    int nr_range;
    struct dev_dax_range *ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    int nr_range;
    struct dev_dax_range *ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    int nr_range;
    struct dev_dax_range *ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    int nr_range;
    struct dev_dax_range *ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    int nr_range;
    struct dev_dax_range *ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    bool dyn_id;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    int nr_range;
    struct dev_dax_range *ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    unsigned int align;
    int target_node;
    bool dyn_id;
    int id;
    struct ida ida;
    struct device dev;
    struct dev_pagemap *pgmap;
    bool memmap_on_memory;
    int nr_range;
    struct dev_dax_range *ranges;
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
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
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
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dev_dax {
    struct dax_region *region;
    struct dax_device *dax_dev;
    int target_node;
    struct device dev;
    struct dev_pagemap pgmap;
    struct resource *dax_kmem_res;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>unsigned int align</code>
</li>
<li>
<b>Field added. </b>
<code>int id</code>
</li>
<li>
<b>Field added. </b>
<code>struct ida ida</code>
</li>
<li>
<b>Field added. </b>
<code>int nr_range</code>
</li>
<li>
<b>Field added. </b>
<code>struct dev_dax_range *ranges</code>
</li>
<li>
<b>Field removed. </b>
<code>struct resource *dax_kmem_res</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dev_pagemap pgmap</code> ➡️ <code>struct dev_pagemap *pgmap</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool dyn_id</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool memmap_on_memory</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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

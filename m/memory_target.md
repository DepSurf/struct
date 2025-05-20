# Struct: <code>memory_target</code>

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
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct node_hmem_attrs hmem_attrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct node_hmem_attrs hmem_attrs;
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs;
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs[2];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs[2];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs[2];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs[2];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs[2];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct node_hmem_attrs hmem_attrs[2];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct resource memregions;
    struct access_coordinate coord[3];
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    u8 gen_port_device_handle[16];
    bool registered;
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
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct node_hmem_attrs hmem_attrs;
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct node_hmem_attrs hmem_attrs;
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct node_hmem_attrs hmem_attrs;
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct memory_target {
    struct list_head node;
    unsigned int memory_pxm;
    unsigned int processor_pxm;
    struct node_hmem_attrs hmem_attrs;
    struct list_head caches;
    struct node_cache_attrs cache_attrs;
    bool registered;
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
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head caches</code>
</li>
<li>
<b>Field added. </b>
<code>struct node_cache_attrs cache_attrs</code>
</li>
<li>
<b>Field added. </b>
<code>bool registered</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct resource memregions</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct node_hmem_attrs hmem_attrs</code> ➡️ <code>struct node_hmem_attrs hmem_attrs[2]</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct access_coordinate coord[3]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 gen_port_device_handle[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct node_hmem_attrs hmem_attrs[2]</code>
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
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

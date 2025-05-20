# Struct: <code>sgx_epc_section</code>

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
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    spinlock_t lock;
    struct list_head page_list;
    long unsigned int free_cnt;
    struct list_head init_laundry_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    struct sgx_numa_node *node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    struct sgx_numa_node *node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    struct sgx_numa_node *node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    struct sgx_numa_node *node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    struct sgx_numa_node *node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sgx_epc_section {
    long unsigned int phys_addr;
    void *virt_addr;
    struct sgx_epc_page *pages;
    struct sgx_numa_node *node;
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
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sgx_numa_node *node</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head page_list</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int free_cnt</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head init_laundry_list</code>
</li>
</ul>
</details>
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

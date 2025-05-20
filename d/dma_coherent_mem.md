# Struct: <code>dma_coherent_mem</code>

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
struct dma_coherent_mem {
    void *virt_base;
    dma_addr_t device_base;
    long unsigned int pfn_base;
    int size;
    long unsigned int *bitmap;
    spinlock_t spinlock;
    bool use_dev_dma_pfn_offset;
};
```
</details>
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
struct dma_coherent_mem {
    void *virt_base;
    dma_addr_t device_base;
    long unsigned int pfn_base;
    int size;
    long unsigned int *bitmap;
    spinlock_t spinlock;
    bool use_dev_dma_pfn_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dma_coherent_mem {
    void *virt_base;
    dma_addr_t device_base;
    long unsigned int pfn_base;
    int size;
    long unsigned int *bitmap;
    spinlock_t spinlock;
    bool use_dev_dma_pfn_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dma_coherent_mem {
    void *virt_base;
    dma_addr_t device_base;
    long unsigned int pfn_base;
    int size;
    long unsigned int *bitmap;
    spinlock_t spinlock;
    bool use_dev_dma_pfn_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dma_coherent_mem {
    void *virt_base;
    dma_addr_t device_base;
    long unsigned int pfn_base;
    int size;
    long unsigned int *bitmap;
    spinlock_t spinlock;
    bool use_dev_dma_pfn_offset;
};
```
</details>
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
</ul>
<b>Arch</b>
<ul>
</ul>

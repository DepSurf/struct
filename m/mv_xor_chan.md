# Struct: <code>mv_xor_chan</code>

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
struct mv_xor_chan {
    int pending;
    spinlock_t lock;
    void *mmr_base;
    void *mmr_high_base;
    unsigned int idx;
    int irq;
    struct list_head chain;
    struct list_head free_slots;
    struct list_head allocated_slots;
    struct list_head completed_slots;
    dma_addr_t dma_desc_pool;
    void *dma_desc_pool_virt;
    size_t pool_size;
    struct dma_device dmadev;
    struct dma_chan dmachan;
    int slots_allocated;
    struct tasklet_struct irq_tasklet;
    int op_in_desc;
    char dummy_src[128];
    char dummy_dst[128];
    dma_addr_t dummy_src_addr;
    dma_addr_t dummy_dst_addr;
    u32 saved_config_reg;
    u32 saved_int_mask_reg;
    struct mv_xor_device *xordev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mv_xor_chan {
    int pending;
    spinlock_t lock;
    void *mmr_base;
    void *mmr_high_base;
    unsigned int idx;
    int irq;
    struct list_head chain;
    struct list_head free_slots;
    struct list_head allocated_slots;
    struct list_head completed_slots;
    dma_addr_t dma_desc_pool;
    void *dma_desc_pool_virt;
    size_t pool_size;
    struct dma_device dmadev;
    struct dma_chan dmachan;
    int slots_allocated;
    struct tasklet_struct irq_tasklet;
    int op_in_desc;
    char dummy_src[128];
    char dummy_dst[128];
    dma_addr_t dummy_src_addr;
    dma_addr_t dummy_dst_addr;
    u32 saved_config_reg;
    u32 saved_int_mask_reg;
    struct mv_xor_device *xordev;
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

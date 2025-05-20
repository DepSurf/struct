# Struct: <code>nvme_dev</code>

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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct nvme_dev {
    struct nvme_queue *queues;
    struct blk_mq_tag_set tagset;
    struct blk_mq_tag_set admin_tagset;
    u32 *dbs;
    struct device *dev;
    struct dma_pool *prp_page_pool;
    struct dma_pool *prp_small_pool;
    unsigned int online_queues;
    unsigned int max_qid;
    unsigned int io_queues[3];
    unsigned int num_vecs;
    int q_depth;
    int io_sqes;
    u32 db_stride;
    void *bar;
    long unsigned int bar_mapped_size;
    struct work_struct remove_work;
    struct mutex shutdown_lock;
    bool subsystem;
    u64 cmb_size;
    bool cmb_use_sqes;
    u32 cmbsz;
    u32 cmbloc;
    struct nvme_ctrl ctrl;
    u32 last_ps;
    mempool_t *iod_mempool;
    u32 *dbbuf_dbs;
    dma_addr_t dbbuf_dbs_dma_addr;
    u32 *dbbuf_eis;
    dma_addr_t dbbuf_eis_dma_addr;
    u64 host_mem_size;
    u32 nr_host_mem_descs;
    dma_addr_t host_mem_descs_dma;
    struct nvme_host_mem_buf_desc *host_mem_descs;
    void **host_mem_desc_bufs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvme_dev {
    struct nvme_queue *queues;
    struct blk_mq_tag_set tagset;
    struct blk_mq_tag_set admin_tagset;
    u32 *dbs;
    struct device *dev;
    struct dma_pool *prp_page_pool;
    struct dma_pool *prp_small_pool;
    unsigned int online_queues;
    unsigned int max_qid;
    unsigned int io_queues[3];
    unsigned int num_vecs;
    int q_depth;
    int io_sqes;
    u32 db_stride;
    void *bar;
    long unsigned int bar_mapped_size;
    struct work_struct remove_work;
    struct mutex shutdown_lock;
    bool subsystem;
    u64 cmb_size;
    bool cmb_use_sqes;
    u32 cmbsz;
    u32 cmbloc;
    struct nvme_ctrl ctrl;
    u32 last_ps;
    mempool_t *iod_mempool;
    u32 *dbbuf_dbs;
    dma_addr_t dbbuf_dbs_dma_addr;
    u32 *dbbuf_eis;
    dma_addr_t dbbuf_eis_dma_addr;
    u64 host_mem_size;
    u32 nr_host_mem_descs;
    dma_addr_t host_mem_descs_dma;
    struct nvme_host_mem_buf_desc *host_mem_descs;
    void **host_mem_desc_bufs;
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Flavor</b>
<ul>
</ul>

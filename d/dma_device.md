# Struct: <code>dma_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    struct mutex chan_mutex;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    struct mutex chan_mutex;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    struct mutex chan_mutex;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    struct mutex chan_mutex;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dma_device {
    struct kref ref;
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    enum dma_desc_metadata_mode desc_metadata_modes;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    struct ida chan_ida;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 min_burst;
    u32 max_burst;
    u32 max_sg_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    int (*device_router_config)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    void (*device_caps)(struct dma_chan *, struct dma_slave_caps *);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
    void (*device_release)(struct dma_device *);
    void (*dbg_summary_show)(struct seq_file *, struct dma_device *);
    struct dentry *dbg_dev_root;
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
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
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
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dma_device {
    unsigned int chancnt;
    unsigned int privatecnt;
    struct list_head channels;
    struct list_head global_node;
    struct dma_filter filter;
    dma_cap_mask_t cap_mask;
    short unsigned int max_xor;
    short unsigned int max_pq;
    enum dmaengine_alignment copy_align;
    enum dmaengine_alignment xor_align;
    enum dmaengine_alignment pq_align;
    enum dmaengine_alignment fill_align;
    int dev_id;
    struct device *dev;
    struct module *owner;
    u32 src_addr_widths;
    u32 dst_addr_widths;
    u32 directions;
    u32 max_burst;
    bool descriptor_reuse;
    enum dma_residue_granularity residue_granularity;
    int (*device_alloc_chan_resources)(struct dma_chan *);
    void (*device_free_chan_resources)(struct dma_chan *);
    struct dma_async_tx_descriptor * (*device_prep_dma_memcpy)(struct dma_chan *, dma_addr_t, dma_addr_t, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor)(struct dma_chan *, dma_addr_t, dma_addr_t *, unsigned int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_xor_val)(struct dma_chan *, dma_addr_t *, unsigned int, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_pq_val)(struct dma_chan *, dma_addr_t *, dma_addr_t *, unsigned int, const unsigned char *, size_t, enum sum_check_flags *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset)(struct dma_chan *, dma_addr_t, int, size_t, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_memset_sg)(struct dma_chan *, struct scatterlist *, unsigned int, int, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_interrupt)(struct dma_chan *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_slave_sg)(struct dma_chan *, struct scatterlist *, unsigned int, enum dma_transfer_direction, long unsigned int, void *);
    struct dma_async_tx_descriptor * (*device_prep_dma_cyclic)(struct dma_chan *, dma_addr_t, size_t, size_t, enum dma_transfer_direction, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_interleaved_dma)(struct dma_chan *, struct dma_interleaved_template *, long unsigned int);
    struct dma_async_tx_descriptor * (*device_prep_dma_imm_data)(struct dma_chan *, dma_addr_t, u64, long unsigned int);
    int (*device_config)(struct dma_chan *, struct dma_slave_config *);
    int (*device_pause)(struct dma_chan *);
    int (*device_resume)(struct dma_chan *);
    int (*device_terminate_all)(struct dma_chan *);
    void (*device_synchronize)(struct dma_chan *);
    enum dma_status (*device_tx_status)(struct dma_chan *, dma_cookie_t, struct dma_tx_state *);
    void (*device_issue_pending)(struct dma_chan *);
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
<code>struct dma_filter filter</code>
</li>
<li>
<b>Field added. </b>
<code>u32 max_burst</code>
</li>
<li>
<b>Field added. </b>
<code>bool descriptor_reuse</code>
</li>
<li>
<b>Field added. </b>
<code>void (*device_synchronize)(struct dma_chan *)</code>
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct dma_async_tx_descriptor * (*device_prep_dma_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct module *owner</code>
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
<code>struct kref ref</code>
</li>
<li>
<b>Field added. </b>
<code>enum dma_desc_metadata_mode desc_metadata_modes</code>
</li>
<li>
<b>Field added. </b>
<code>struct ida chan_ida</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex chan_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>void (*device_release)(struct dma_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*dbg_summary_show)(struct seq_file *, struct dma_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct dentry *dbg_dev_root</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 min_burst</code>
</li>
<li>
<b>Field added. </b>
<code>u32 max_sg_burst</code>
</li>
<li>
<b>Field added. </b>
<code>int (*device_router_config)(struct dma_chan *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*device_caps)(struct dma_chan *, struct dma_slave_caps *)</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dma_async_tx_descriptor * (*device_prep_dma_memcpy_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex chan_mutex</code>
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
<code>struct dma_async_tx_descriptor * (*device_prep_dma_memcpy_sg)(struct dma_chan *, struct scatterlist *, unsigned int, struct scatterlist *, unsigned int, long unsigned int)</code>
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

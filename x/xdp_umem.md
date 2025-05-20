# Struct: <code>xdp_umem</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    struct xdp_umem_props props;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    struct pid *pid;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    struct net_device *dev;
    u16 queue_id;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    struct pid *pid;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    u16 queue_id;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    u16 queue_id;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xsk_buff_pool *pool;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    struct user_struct *user;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    bool zc;
    spinlock_t xsk_tx_list_lock;
    struct list_head xsk_tx_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xdp_umem {
    void *addrs;
    u64 size;
    u32 headroom;
    u32 chunk_size;
    u32 chunks;
    u32 npgs;
    struct user_struct *user;
    refcount_t users;
    u8 flags;
    u8 tx_metadata_len;
    bool zc;
    struct page **pgs;
    int id;
    struct list_head xsk_dma_list;
    struct work_struct work;
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
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
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
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xdp_umem {
    struct xsk_queue *fq;
    struct xsk_queue *cq;
    struct xdp_umem_page *pages;
    u64 chunk_mask;
    u64 size;
    u32 headroom;
    u32 chunk_size_nohr;
    struct user_struct *user;
    long unsigned int address;
    refcount_t users;
    struct work_struct work;
    struct page **pgs;
    u32 npgs;
    u16 queue_id;
    u8 need_wakeup;
    u8 flags;
    int id;
    struct net_device *dev;
    struct xdp_umem_fq_reuse *fq_reuse;
    bool zc;
    spinlock_t xsk_list_lock;
    struct list_head xsk_list;
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
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 chunk_mask</code>
</li>
<li>
<b>Field added. </b>
<code>u64 size</code>
</li>
<li>
<b>Field added. </b>
<code>struct xdp_umem_fq_reuse *fq_reuse</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xdp_umem_props props</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int id</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pid *pid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 need_wakeup</code>
</li>
<li>
<b>Field added. </b>
<code>u8 flags</code>
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
<code>struct xsk_buff_pool *pool</code>
</li>
<li>
<b>Field added. </b>
<code>u32 chunk_size</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t xsk_tx_list_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head xsk_tx_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xdp_umem_page *pages</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 chunk_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 chunk_size_nohr</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int address</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xdp_umem_fq_reuse *fq_reuse</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t xsk_list_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head xsk_list</code>
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
<code>void *addrs</code>
</li>
<li>
<b>Field added. </b>
<code>u32 chunks</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head xsk_dma_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xsk_queue *fq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xsk_queue *cq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xsk_buff_pool *pool</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 queue_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 need_wakeup</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device *dev</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t xsk_tx_list_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head xsk_tx_list</code>
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
<code>u8 tx_metadata_len</code>
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

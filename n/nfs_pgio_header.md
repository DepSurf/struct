# Struct: <code>nfs_pgio_header</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    struct rpc_cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_direct_req *dreq;
    void *layout_private;
    spinlock_t lock;
    int pnfs_error;
    int error;
    long unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    struct rpc_cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_direct_req *dreq;
    void *layout_private;
    spinlock_t lock;
    int pnfs_error;
    int error;
    long unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    struct rpc_cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    spinlock_t lock;
    int pnfs_error;
    int error;
    long unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    struct rpc_cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    spinlock_t lock;
    int pnfs_error;
    int error;
    long unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    struct rpc_cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    spinlock_t lock;
    int pnfs_error;
    int error;
    long unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    u32 ds_commit_idx;
    u32 pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    u32 ds_commit_idx;
    u32 pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    u32 ds_commit_idx;
    u32 pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    u32 ds_commit_idx;
    u32 pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    void *netfs;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    u32 ds_commit_idx;
    u32 pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    void *netfs;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    u32 ds_commit_idx;
    u32 pgio_mirror_idx;
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
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
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
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nfs_pgio_header {
    struct inode *inode;
    const struct cred *cred;
    struct list_head pages;
    struct nfs_page *req;
    struct nfs_writeverf verf;
    fmode_t rw_mode;
    struct pnfs_layout_segment *lseg;
    loff_t io_start;
    const struct rpc_call_ops *mds_ops;
    void (*release)(struct nfs_pgio_header *);
    const struct nfs_pgio_completion_ops *completion_ops;
    const struct nfs_rw_ops *rw_ops;
    struct nfs_io_completion *io_completion;
    struct nfs_direct_req *dreq;
    int pnfs_error;
    int error;
    unsigned int good_bytes;
    long unsigned int flags;
    struct rpc_task task;
    struct nfs_fattr fattr;
    struct nfs_pgio_args args;
    struct nfs_pgio_res res;
    long unsigned int timestamp;
    int (*pgio_done_cb)(struct rpc_task *, struct nfs_pgio_header *);
    __u64 mds_offset;
    struct nfs_page_array page_array;
    struct nfs_client *ds_clp;
    int ds_commit_idx;
    int pgio_mirror_idx;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>fmode_t rw_mode</code>
</li>
<li>
<b>Field added. </b>
<code>struct nfs_io_completion *io_completion</code>
</li>
<li>
<b>Field removed. </b>
<code>void *layout_private</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rpc_cred *cred</code> ➡️ <code>const struct cred *cred</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int good_bytes</code> ➡️ <code>unsigned int good_bytes</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
<code>void *netfs</code>
</li>
</ul>
</details>
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

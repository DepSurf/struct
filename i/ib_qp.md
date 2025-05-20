# Struct: <code>ib_qp</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u32 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u32 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u32 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u32 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u32 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uqp_object *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u32 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
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
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
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
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ib_qp {
    struct ib_device *device;
    struct ib_pd *pd;
    struct ib_cq *send_cq;
    struct ib_cq *recv_cq;
    spinlock_t mr_lock;
    int mrs_used;
    struct list_head rdma_mrs;
    struct list_head sig_mrs;
    struct ib_srq *srq;
    struct ib_xrcd *xrcd;
    struct list_head xrcd_list;
    atomic_t usecnt;
    struct list_head open_list;
    struct ib_qp *real_qp;
    struct ib_uobject *uobject;
    void (*event_handler)(struct ib_event *, void *);
    void *qp_context;
    const struct ib_gid_attr *av_sgid_attr;
    const struct ib_gid_attr *alt_path_sgid_attr;
    u32 qp_num;
    u32 max_write_sge;
    u32 max_read_sge;
    enum ib_qp_type qp_type;
    struct ib_rwq_ind_table *rwq_ind_tbl;
    struct ib_qp_security *qp_sec;
    u8 port;
    bool integrity_en;
    struct rdma_restrack_entry res;
    struct rdma_counter *counter;
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rdma_restrack_entry res</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct ib_gid_attr *av_sgid_attr</code>
</li>
<li>
<b>Field added. </b>
<code>const struct ib_gid_attr *alt_path_sgid_attr</code>
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
<code>bool integrity_en</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdma_counter *counter</code>
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
<b>Field type changed. </b>
<code>struct ib_uobject *uobject</code> ➡️ <code>struct ib_uqp_object *uobject</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 port</code> ➡️ <code>u32 port</code>
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

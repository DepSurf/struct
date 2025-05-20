# Struct: <code>ib_cq</code>

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
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_ucq_object *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    unsigned int cqe_used;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct list_head pool_entry;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    ktime_t timestamp;
    u8 interrupt;
    u8 shared;
    unsigned int comp_vector;
    struct rdma_restrack_entry res;
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
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
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
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ib_cq {
    struct ib_device *device;
    struct ib_uobject *uobject;
    ib_comp_handler comp_handler;
    void (*event_handler)(struct ib_event *, void *);
    void *cq_context;
    int cqe;
    atomic_t usecnt;
    enum ib_poll_context poll_ctx;
    struct ib_wc *wc;
    struct irq_poll iop;
    struct work_struct work;
    struct workqueue_struct *comp_wq;
    struct dim *dim;
    struct rdma_restrack_entry res;
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
<code>struct workqueue_struct *comp_wq</code>
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
<code>struct dim *dim</code>
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
<b>Field added. </b>
<code>unsigned int cqe_used</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head pool_entry</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t timestamp</code>
</li>
<li>
<b>Field added. </b>
<code>u8 interrupt</code>
</li>
<li>
<b>Field added. </b>
<code>u8 shared</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int comp_vector</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_uobject *uobject</code> ➡️ <code>struct ib_ucq_object *uobject</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
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

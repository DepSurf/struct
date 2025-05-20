# Struct: <code>spu</code>

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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spu {
    const char *name;
    long unsigned int local_store_phys;
    u8 *local_store;
    long unsigned int problem_phys;
    struct spu_problem *problem;
    struct spu_priv2 *priv2;
    struct list_head cbe_list;
    struct list_head full_list;
    enum (anon) alloc_state;
    int number;
    unsigned int irqs[3];
    u32 node;
    long unsigned int flags;
    u64 class_0_pending;
    u64 class_0_dar;
    u64 class_1_dar;
    u64 class_1_dsisr;
    size_t ls_size;
    unsigned int slb_replace;
    struct mm_struct *mm;
    struct spu_context *ctx;
    struct spu_runqueue *rq;
    long long unsigned int timestamp;
    pid_t pid;
    pid_t tgid;
    spinlock_t register_lock;
    void (*wbox_callback)(struct spu *);
    void (*ibox_callback)(struct spu *);
    void (*stop_callback)(struct spu *, int);
    void (*mfc_callback)(struct spu *);
    char irq_c0[8];
    char irq_c1[8];
    char irq_c2[8];
    u64 spe_id;
    void *pdata;
    struct device_node *devnode;
    struct spu_priv1 *priv1;
    u64 shadow_int_mask_RW[3];
    struct device dev;
    int has_mem_affinity;
    struct list_head aff_list;
    struct (anon) stats;
};
```
</details>
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

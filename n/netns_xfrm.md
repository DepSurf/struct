# Struct: <code>netns_xfrm</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct hlist_head state_gc_list;
    struct work_struct state_gc_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    rwlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
    struct flow_cache flow_cache_global;
    atomic_t flow_cache_genid;
    struct list_head flow_cache_gc_list;
    spinlock_t flow_cache_gc_lock;
    struct work_struct flow_cache_gc_work;
    struct work_struct flow_cache_flush_work;
    struct mutex flow_flush_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct hlist_head state_gc_list;
    struct work_struct state_gc_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    rwlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
    struct flow_cache flow_cache_global;
    atomic_t flow_cache_genid;
    struct list_head flow_cache_gc_list;
    atomic_t flow_cache_gc_count;
    spinlock_t flow_cache_gc_lock;
    struct work_struct flow_cache_gc_work;
    struct work_struct flow_cache_flush_work;
    struct mutex flow_flush_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
    struct flow_cache flow_cache_global;
    atomic_t flow_cache_genid;
    struct list_head flow_cache_gc_list;
    atomic_t flow_cache_gc_count;
    spinlock_t flow_cache_gc_lock;
    struct work_struct flow_cache_gc_work;
    struct work_struct flow_cache_flush_work;
    struct mutex flow_flush_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
    struct flow_cache flow_cache_global;
    atomic_t flow_cache_genid;
    struct list_head flow_cache_gc_list;
    atomic_t flow_cache_gc_count;
    spinlock_t flow_cache_gc_lock;
    struct work_struct flow_cache_gc_work;
    struct work_struct flow_cache_flush_work;
    struct mutex flow_flush_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    seqcount_spinlock_t xfrm_state_hash_generation;
    seqcount_spinlock_t xfrm_policy_hash_generation;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    struct hlist_head *state_byseq;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    u8 policy_default;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    seqcount_spinlock_t xfrm_state_hash_generation;
    seqcount_spinlock_t xfrm_policy_hash_generation;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    struct hlist_head *state_byseq;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    u8 policy_default[3];
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    seqcount_spinlock_t xfrm_state_hash_generation;
    seqcount_spinlock_t xfrm_policy_hash_generation;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    struct hlist_head *state_byseq;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    u8 policy_default[3];
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    seqcount_spinlock_t xfrm_state_hash_generation;
    seqcount_spinlock_t xfrm_policy_hash_generation;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    struct hlist_head *state_byseq;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    u8 policy_default[3];
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    seqcount_spinlock_t xfrm_state_hash_generation;
    seqcount_spinlock_t xfrm_policy_hash_generation;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    struct hlist_head *state_byseq;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    unsigned int idx_generator;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    u8 policy_default[3];
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    seqcount_spinlock_t xfrm_state_hash_generation;
    seqcount_spinlock_t xfrm_policy_hash_generation;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
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
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
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
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_xfrm {
    struct list_head state_all;
    struct hlist_head *state_bydst;
    struct hlist_head *state_bysrc;
    struct hlist_head *state_byspi;
    unsigned int state_hmask;
    unsigned int state_num;
    struct work_struct state_hash_work;
    struct list_head policy_all;
    struct hlist_head *policy_byidx;
    unsigned int policy_idx_hmask;
    struct hlist_head policy_inexact[3];
    struct xfrm_policy_hash policy_bydst[3];
    unsigned int policy_count[6];
    struct work_struct policy_hash_work;
    struct xfrm_policy_hthresh policy_hthresh;
    struct list_head inexact_bins;
    struct sock *nlsk;
    struct sock *nlsk_stash;
    u32 sysctl_aevent_etime;
    u32 sysctl_aevent_rseqth;
    int sysctl_larval_drop;
    u32 sysctl_acq_expires;
    struct ctl_table_header *sysctl_hdr;
    struct dst_ops xfrm4_dst_ops;
    struct dst_ops xfrm6_dst_ops;
    spinlock_t xfrm_state_lock;
    spinlock_t xfrm_policy_lock;
    struct mutex xfrm_cfg_mutex;
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
<code>atomic_t flow_cache_gc_count</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct hlist_head state_gc_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct state_gc_work</code>
</li>
<li>
<b>Field type changed. </b>
<code>rwlock_t xfrm_policy_lock</code> ➡️ <code>spinlock_t xfrm_policy_lock</code>
</li>
</ul>
</details>
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
<code>struct flow_cache flow_cache_global</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t flow_cache_genid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head flow_cache_gc_list</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t flow_cache_gc_count</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t flow_cache_gc_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct flow_cache_gc_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct flow_cache_flush_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex flow_flush_sem</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head inexact_bins</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>seqcount_spinlock_t xfrm_state_hash_generation</code>
</li>
<li>
<b>Field added. </b>
<code>seqcount_spinlock_t xfrm_policy_hash_generation</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_head *state_byseq</code>
</li>
<li>
<b>Field added. </b>
<code>u8 policy_default</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 policy_default</code> ➡️ <code>u8 policy_default[3]</code>
</li>
</ul>
</details>
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
<code>unsigned int idx_generator</code>
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

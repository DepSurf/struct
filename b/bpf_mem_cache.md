# Struct: <code>bpf_mem_cache</code>

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
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_mem_cache {
    struct llist_head free_llist;
    local_t active;
    struct llist_head free_llist_extra;
    struct irq_work refill_work;
    struct obj_cgroup *objcg;
    int unit_size;
    int free_cnt;
    int low_watermark;
    int high_watermark;
    int batch;
    int percpu_size;
    struct callback_head rcu;
    struct llist_head free_by_rcu;
    struct llist_head waiting_for_gp;
    atomic_t call_rcu_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_mem_cache {
    struct llist_head free_llist;
    local_t active;
    struct llist_head free_llist_extra;
    struct irq_work refill_work;
    struct obj_cgroup *objcg;
    int unit_size;
    int free_cnt;
    int low_watermark;
    int high_watermark;
    int batch;
    int percpu_size;
    struct callback_head rcu;
    struct llist_head free_by_rcu;
    struct llist_head waiting_for_gp;
    atomic_t call_rcu_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_mem_cache {
    struct llist_head free_llist;
    local_t active;
    struct llist_head free_llist_extra;
    struct irq_work refill_work;
    struct obj_cgroup *objcg;
    int unit_size;
    int free_cnt;
    int low_watermark;
    int high_watermark;
    int batch;
    int percpu_size;
    bool draining;
    struct bpf_mem_cache *tgt;
    struct llist_head free_by_rcu;
    struct llist_node *free_by_rcu_tail;
    struct llist_head waiting_for_gp;
    struct llist_node *waiting_for_gp_tail;
    struct callback_head rcu;
    atomic_t call_rcu_in_progress;
    struct llist_head free_llist_extra_rcu;
    struct llist_head free_by_rcu_ttrace;
    struct llist_head waiting_for_gp_ttrace;
    struct callback_head rcu_ttrace;
    atomic_t call_rcu_ttrace_in_progress;
};
```
</details>
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
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool draining</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_mem_cache *tgt</code>
</li>
<li>
<b>Field added. </b>
<code>struct llist_node *free_by_rcu_tail</code>
</li>
<li>
<b>Field added. </b>
<code>struct llist_node *waiting_for_gp_tail</code>
</li>
<li>
<b>Field added. </b>
<code>struct llist_head free_llist_extra_rcu</code>
</li>
<li>
<b>Field added. </b>
<code>struct llist_head free_by_rcu_ttrace</code>
</li>
<li>
<b>Field added. </b>
<code>struct llist_head waiting_for_gp_ttrace</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu_ttrace</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t call_rcu_ttrace_in_progress</code>
</li>
</ul>
</details>
</li>
</ul>

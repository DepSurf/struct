# Struct: <code>css_set</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct css_set {
    atomic_t refcount;
    struct hlist_node hlist;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head cgrp_links;
    struct cgroup *dfl_cgrp;
    struct cgroup_subsys_state * subsys[12];
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct css_set *mg_dst_cset;
    struct list_head e_cset_node[12];
    struct list_head task_iters;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct css_set {
    atomic_t refcount;
    struct hlist_node hlist;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head cgrp_links;
    struct cgroup *dfl_cgrp;
    struct cgroup_subsys_state * subsys[12];
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    struct list_head e_cset_node[12];
    struct list_head task_iters;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct css_set {
    atomic_t refcount;
    struct hlist_node hlist;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head cgrp_links;
    struct cgroup *dfl_cgrp;
    struct cgroup_subsys_state * subsys[12];
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    struct list_head e_cset_node[12];
    struct list_head task_iters;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[14];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[14];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[14];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[14];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[14];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[14];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_src_preload_node;
    struct list_head mg_dst_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[14];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[14];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_src_preload_node;
    struct list_head mg_dst_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[14];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[14];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_src_preload_node;
    struct list_head mg_dst_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[14];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[14];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_src_preload_node;
    struct list_head mg_dst_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
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
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[12];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[12];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
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
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct css_set {
    struct cgroup_subsys_state * subsys[13];
    refcount_t refcount;
    struct css_set *dom_cset;
    struct cgroup *dfl_cgrp;
    int nr_tasks;
    struct list_head tasks;
    struct list_head mg_tasks;
    struct list_head dying_tasks;
    struct list_head task_iters;
    struct list_head e_cset_node[13];
    struct list_head threaded_csets;
    struct list_head threaded_csets_node;
    struct hlist_node hlist;
    struct list_head cgrp_links;
    struct list_head mg_preload_node;
    struct list_head mg_node;
    struct cgroup *mg_src_cgrp;
    struct cgroup *mg_dst_cgrp;
    struct css_set *mg_dst_cset;
    bool dead;
    struct callback_head callback_head;
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
<code>struct cgroup *mg_dst_cgrp</code>
</li>
<li>
<b>Field added. </b>
<code>bool dead</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int nr_tasks</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t refcount</code> ➡️ <code>refcount_t refcount</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct cgroup_subsys_state * subsys[12]</code> ➡️ <code>struct cgroup_subsys_state * subsys[13]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head e_cset_node[12]</code> ➡️ <code>struct list_head e_cset_node[13]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct css_set *dom_cset</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head threaded_csets</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head threaded_csets_node</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head dying_tasks</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>struct cgroup_subsys_state * subsys[13]</code> ➡️ <code>struct cgroup_subsys_state * subsys[14]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head e_cset_node[13]</code> ➡️ <code>struct list_head e_cset_node[14]</code>
</li>
</ul>
</details>
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
<code>struct list_head mg_src_preload_node</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head mg_dst_preload_node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head mg_preload_node</code>
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct cgroup_subsys_state * subsys[13]</code> ➡️ <code>struct cgroup_subsys_state * subsys[12]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head e_cset_node[13]</code> ➡️ <code>struct list_head e_cset_node[12]</code>
</li>
</ul>
</details>
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

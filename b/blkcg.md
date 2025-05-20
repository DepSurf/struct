# Struct: <code>blkcg</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct radix_tree_root blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[2];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct radix_tree_root blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[2];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct radix_tree_root blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[2];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct radix_tree_root blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[3];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct radix_tree_root blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[3];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct radix_tree_root blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[3];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[6];
    struct list_head all_blkcgs_node;
    char fc_app_id[129];
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[6];
    struct list_head all_blkcgs_node;
    char fc_app_id[129];
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[6];
    struct list_head all_blkcgs_node;
    struct llist_head *lhead;
    char fc_app_id[129];
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[6];
    struct list_head all_blkcgs_node;
    struct llist_head *lhead;
    char fc_app_id[129];
    struct list_head cgwb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    refcount_t online_pin;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[6];
    struct list_head all_blkcgs_node;
    struct llist_head *lhead;
    char fc_app_id[129];
    struct list_head cgwb_list;
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
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
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
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blkcg {
    struct cgroup_subsys_state css;
    spinlock_t lock;
    struct xarray blkg_tree;
    struct blkcg_gq *blkg_hint;
    struct hlist_head blkg_list;
    struct blkcg_policy_data * cpd[5];
    struct list_head all_blkcgs_node;
    struct list_head cgwb_list;
    refcount_t cgwb_refcnt;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct blkcg_policy_data * cpd[2]</code> ➡️ <code>struct blkcg_policy_data * cpd[3]</code>
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
<b>Field added. </b>
<code>refcount_t cgwb_refcnt</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct radix_tree_root blkg_tree</code> ➡️ <code>struct xarray blkg_tree</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct blkcg_policy_data * cpd[3]</code> ➡️ <code>struct blkcg_policy_data * cpd[5]</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>refcount_t online_pin</code>
</li>
<li>
<b>Field removed. </b>
<code>refcount_t cgwb_refcnt</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>char fc_app_id[129]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct blkcg_policy_data * cpd[5]</code> ➡️ <code>struct blkcg_policy_data * cpd[6]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct llist_head *lhead</code>
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

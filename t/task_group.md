# Struct: <code>task_group</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    int idle;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    int idle;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    int idle;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    int idle;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    int idle;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
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
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
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
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct sched_rt_entity **rt_se;
    struct rt_rq **rt_rq;
    struct rt_bandwidth rt_bandwidth;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct task_group {
    struct cgroup_subsys_state css;
    struct sched_entity **se;
    struct cfs_rq **cfs_rq;
    long unsigned int shares;
    atomic_long_t load_avg;
    struct callback_head rcu;
    struct list_head list;
    struct task_group *parent;
    struct list_head siblings;
    struct list_head children;
    struct autogroup *autogroup;
    struct cfs_bandwidth cfs_bandwidth;
    unsigned int uclamp_pct[2];
    struct uclamp_se uclamp_req[2];
    struct uclamp_se uclamp[2];
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
<code>struct sched_rt_entity **rt_se</code>
</li>
<li>
<b>Field added. </b>
<code>struct rt_rq **rt_rq</code>
</li>
<li>
<b>Field added. </b>
<code>struct rt_bandwidth rt_bandwidth</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int uclamp_pct[2]</code>
</li>
<li>
<b>Field added. </b>
<code>struct uclamp_se uclamp_req[2]</code>
</li>
<li>
<b>Field added. </b>
<code>struct uclamp_se uclamp[2]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct sched_rt_entity **rt_se</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt_rq **rt_rq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt_bandwidth rt_bandwidth</code>
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
<code>int idle</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int uclamp_pct[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uclamp_se uclamp_req[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uclamp_se uclamp[2]</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct sched_rt_entity **rt_se</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt_rq **rt_rq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt_bandwidth rt_bandwidth</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>gcp</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int uclamp_pct[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uclamp_se uclamp_req[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uclamp_se uclamp[2]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>lowlatency</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct sched_rt_entity **rt_se</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt_rq **rt_rq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt_bandwidth rt_bandwidth</code>
</li>
</ul>
</details>
</li>
</ul>

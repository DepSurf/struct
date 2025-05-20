# Struct: <code>sched_dl_entity</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    int dl_throttled;
    int dl_new;
    int dl_boosted;
    int dl_yielded;
    struct hrtimer dl_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    int dl_throttled;
    int dl_boosted;
    int dl_yielded;
    struct hrtimer dl_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    int dl_throttled;
    int dl_boosted;
    int dl_yielded;
    struct hrtimer dl_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    int dl_throttled;
    int dl_boosted;
    int dl_yielded;
    int dl_non_contending;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct sched_dl_entity *pi_se;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct sched_dl_entity *pi_se;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct sched_dl_entity *pi_se;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct sched_dl_entity *pi_se;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct sched_dl_entity *pi_se;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct sched_dl_entity *pi_se;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    unsigned int dl_server;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
    struct rq *rq;
    dl_server_has_tasks_f server_has_tasks;
    dl_server_pick_f server_pick;
    struct sched_dl_entity *pi_se;
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
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
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
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sched_dl_entity {
    struct rb_node rb_node;
    u64 dl_runtime;
    u64 dl_deadline;
    u64 dl_period;
    u64 dl_bw;
    u64 dl_density;
    s64 runtime;
    u64 deadline;
    unsigned int flags;
    unsigned int dl_throttled;
    unsigned int dl_boosted;
    unsigned int dl_yielded;
    unsigned int dl_non_contending;
    unsigned int dl_overrun;
    struct hrtimer dl_timer;
    struct hrtimer inactive_timer;
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
<b>Field removed. </b>
<code>int dl_new</code>
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
<code>u64 dl_density</code>
</li>
<li>
<b>Field added. </b>
<code>int dl_non_contending</code>
</li>
<li>
<b>Field added. </b>
<code>struct hrtimer inactive_timer</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int dl_throttled</code> ➡️ <code>unsigned int dl_throttled</code>
</li>
<li>
<b>Field type changed. </b>
<code>int dl_boosted</code> ➡️ <code>unsigned int dl_boosted</code>
</li>
<li>
<b>Field type changed. </b>
<code>int dl_yielded</code> ➡️ <code>unsigned int dl_yielded</code>
</li>
<li>
<b>Field type changed. </b>
<code>int dl_non_contending</code> ➡️ <code>unsigned int dl_non_contending</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int dl_overrun</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sched_dl_entity *pi_se</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int dl_boosted</code>
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
<code>unsigned int dl_server</code>
</li>
<li>
<b>Field added. </b>
<code>struct rq *rq</code>
</li>
<li>
<b>Field added. </b>
<code>dl_server_has_tasks_f server_has_tasks</code>
</li>
<li>
<b>Field added. </b>
<code>dl_server_pick_f server_pick</code>
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

# Struct: <code>dl_rq</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root rb_root;
    struct rb_node *rb_leftmost;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root pushable_dl_tasks_root;
    struct rb_node *pushable_dl_tasks_leftmost;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root rb_root;
    struct rb_node *rb_leftmost;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root pushable_dl_tasks_root;
    struct rb_node *pushable_dl_tasks_leftmost;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root rb_root;
    struct rb_node *rb_leftmost;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root pushable_dl_tasks_root;
    struct rb_node *pushable_dl_tasks_leftmost;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root rb_root;
    struct rb_node *rb_leftmost;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root pushable_dl_tasks_root;
    struct rb_node *pushable_dl_tasks_leftmost;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 max_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 max_bw;
    u64 bw_ratio;
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
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
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
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dl_rq {
    struct rb_root_cached root;
    long unsigned int dl_nr_running;
    struct (anon) earliest_dl;
    long unsigned int dl_nr_migratory;
    int overloaded;
    struct rb_root_cached pushable_dl_tasks_root;
    u64 running_bw;
    u64 this_bw;
    u64 extra_bw;
    u64 bw_ratio;
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
<b>Field added. </b>
<code>u64 running_bw</code>
</li>
<li>
<b>Field added. </b>
<code>u64 this_bw</code>
</li>
<li>
<b>Field added. </b>
<code>u64 extra_bw</code>
</li>
<li>
<b>Field added. </b>
<code>u64 bw_ratio</code>
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
<code>struct rb_root_cached root</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_root rb_root</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_node *rb_leftmost</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_node *pushable_dl_tasks_leftmost</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rb_root pushable_dl_tasks_root</code> ➡️ <code>struct rb_root_cached pushable_dl_tasks_root</code>
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int dl_nr_running</code> ➡️ <code>unsigned int dl_nr_running</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int dl_nr_migratory</code> ➡️ <code>unsigned int dl_nr_migratory</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 max_bw</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int dl_nr_migratory</code>
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

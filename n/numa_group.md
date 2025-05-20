# Struct: <code>numa_group</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    struct callback_head rcu;
    nodemask_t active_nodes;
    long unsigned int total_faults;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct numa_group {
    atomic_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int faults[0];
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
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct numa_group {
    refcount_t refcount;
    spinlock_t lock;
    int nr_tasks;
    pid_t gid;
    int active_nodes;
    struct callback_head rcu;
    long unsigned int total_faults;
    long unsigned int max_faults_cpu;
    long unsigned int *faults_cpu;
    long unsigned int faults[0];
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
<code>long unsigned int max_faults_cpu</code>
</li>
<li>
<b>Field type changed. </b>
<code>nodemask_t active_nodes</code> ➡️ <code>int active_nodes</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t refcount</code> ➡️ <code>refcount_t refcount</code>
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int *faults_cpu</code>
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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

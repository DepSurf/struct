# Struct: <code>srcu_data</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    raw_spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct delayed_work work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *sp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    raw_spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct delayed_work work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *sp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct delayed_work work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *sp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct delayed_work work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct srcu_data {
    atomic_long_t srcu_lock_count[2];
    atomic_long_t srcu_unlock_count[2];
    int srcu_nmi_safety;
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct srcu_data {
    atomic_long_t srcu_lock_count[2];
    atomic_long_t srcu_unlock_count[2];
    int srcu_nmi_safety;
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct srcu_data {
    atomic_long_t srcu_lock_count[2];
    atomic_long_t srcu_unlock_count[2];
    int srcu_nmi_safety;
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
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
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
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
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct srcu_data {
    long unsigned int srcu_lock_count[2];
    long unsigned int srcu_unlock_count[2];
    spinlock_t lock;
    struct rcu_segcblist srcu_cblist;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    bool srcu_cblist_invoking;
    struct timer_list delay_work;
    struct work_struct work;
    struct callback_head srcu_barrier_head;
    struct srcu_node *mynode;
    long unsigned int grpmask;
    int cpu;
    struct srcu_struct *ssp;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>raw_spinlock_t lock</code> ➡️ <code>spinlock_t lock</code>
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
<code>struct srcu_struct *ssp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct srcu_struct *sp</code>
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
<code>struct timer_list delay_work</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct delayed_work work</code> ➡️ <code>struct work_struct work</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int srcu_nmi_safety</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int srcu_lock_count[2]</code> ➡️ <code>atomic_long_t srcu_lock_count[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int srcu_unlock_count[2]</code> ➡️ <code>atomic_long_t srcu_unlock_count[2]</code>
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

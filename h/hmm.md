# Struct: <code>hmm</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hmm {
    struct mm_struct *mm;
    spinlock_t lock;
    atomic_t sequence;
    struct list_head ranges;
    struct list_head mirrors;
    struct mmu_notifier mmu_notifier;
    struct rw_semaphore mirrors_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hmm {
    struct mm_struct *mm;
    spinlock_t lock;
    atomic_t sequence;
    struct list_head ranges;
    struct list_head mirrors;
    struct mmu_notifier mmu_notifier;
    struct rw_semaphore mirrors_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hmm {
    struct mm_struct *mm;
    spinlock_t lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct mmu_notifier mmu_notifier;
    struct rw_semaphore mirrors_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hmm {
    struct mm_struct *mm;
    struct kref kref;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct mmu_notifier mmu_notifier;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    struct callback_head rcu;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
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
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hmm {
    struct mmu_notifier mmu_notifier;
    spinlock_t ranges_lock;
    struct list_head ranges;
    struct list_head mirrors;
    struct rw_semaphore mirrors_sem;
    wait_queue_head_t wq;
    long int notifiers;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t sequence</code>
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
<code>struct kref kref</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t ranges_lock</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t wq</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field added. </b>
<code>long int notifiers</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mm_struct *mm</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kref kref</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head rcu</code>
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

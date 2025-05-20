# Struct: <code>task_delay_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct task_delay_info {
    spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u32 freepages_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct task_delay_info {
    spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u32 freepages_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct task_delay_info {
    spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u32 freepages_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct task_delay_info {
    spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u32 freepages_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct task_delay_info {
    spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u32 freepages_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u32 freepages_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_start;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u64 compact_start;
    u64 compact_delay;
    u64 wpcopy_start;
    u64 wpcopy_delay;
    u32 freepages_count;
    u32 thrashing_count;
    u32 compact_count;
    u32 wpcopy_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_start;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u64 compact_start;
    u64 compact_delay;
    u64 wpcopy_start;
    u64 wpcopy_delay;
    u32 freepages_count;
    u32 thrashing_count;
    u32 compact_count;
    u32 wpcopy_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_start;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u64 compact_start;
    u64 compact_delay;
    u64 wpcopy_start;
    u64 wpcopy_delay;
    u64 irq_delay;
    u32 freepages_count;
    u32 thrashing_count;
    u32 compact_count;
    u32 wpcopy_count;
    u32 irq_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_start;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u64 compact_start;
    u64 compact_delay;
    u64 wpcopy_start;
    u64 wpcopy_delay;
    u64 irq_delay;
    u32 freepages_count;
    u32 thrashing_count;
    u32 compact_count;
    u32 wpcopy_count;
    u32 irq_count;
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
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
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
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct task_delay_info {
    raw_spinlock_t lock;
    unsigned int flags;
    u64 blkio_start;
    u64 blkio_delay;
    u64 swapin_delay;
    u32 blkio_count;
    u32 swapin_count;
    u64 freepages_start;
    u64 freepages_delay;
    u64 thrashing_start;
    u64 thrashing_delay;
    u32 freepages_count;
    u32 thrashing_count;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
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
<code>u64 thrashing_start</code>
</li>
<li>
<b>Field added. </b>
<code>u64 thrashing_delay</code>
</li>
<li>
<b>Field added. </b>
<code>u32 thrashing_count</code>
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
<b>Field added. </b>
<code>u64 swapin_start</code>
</li>
<li>
<b>Field added. </b>
<code>u64 compact_start</code>
</li>
<li>
<b>Field added. </b>
<code>u64 compact_delay</code>
</li>
<li>
<b>Field added. </b>
<code>u64 wpcopy_start</code>
</li>
<li>
<b>Field added. </b>
<code>u64 wpcopy_delay</code>
</li>
<li>
<b>Field added. </b>
<code>u32 compact_count</code>
</li>
<li>
<b>Field added. </b>
<code>u32 wpcopy_count</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
</li>
</ul>
</details>
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
<code>u64 irq_delay</code>
</li>
<li>
<b>Field added. </b>
<code>u32 irq_count</code>
</li>
</ul>
</details>
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

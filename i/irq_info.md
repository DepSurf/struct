# Struct: <code>irq_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    spinlock_t lock;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    raw_spinlock_t lock;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    raw_spinlock_t lock;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    raw_spinlock_t lock;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    raw_spinlock_t lock;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    raw_spinlock_t lock;
    bool is_static;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    struct list_head eoi_list;
    struct rcu_work rwork;
    short int refcnt;
    u8 spurious_cnt;
    u8 is_accounted;
    short int type;
    u8 mask_reason;
    u8 is_active;
    unsigned int irq;
    evtchn_port_t evtchn;
    short unsigned int cpu;
    short unsigned int eoi_cpu;
    unsigned int irq_epoch;
    u64 eoi_time;
    raw_spinlock_t lock;
    bool is_static;
    union (anon) u;
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
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct irq_info {
    struct hlist_node node;
    int irq;
    spinlock_t lock;
    struct list_head *head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct irq_info {
    struct hlist_node node;
    int irq;
    spinlock_t lock;
    struct list_head *head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct irq_info {
    struct hlist_node node;
    int irq;
    spinlock_t lock;
    struct list_head *head;
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
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct irq_info {
    struct hlist_node node;
    int irq;
    spinlock_t lock;
    struct list_head *head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct irq_info {
    struct list_head list;
    int refcnt;
    enum xen_irq_type type;
    unsigned int irq;
    unsigned int evtchn;
    short unsigned int cpu;
    union (anon) u;
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int evtchn</code> ➡️ <code>evtchn_port_t evtchn</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head eoi_list</code>
</li>
<li>
<b>Field added. </b>
<code>u8 spurious_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>u8 is_accounted</code>
</li>
<li>
<b>Field added. </b>
<code>u8 mask_reason</code>
</li>
<li>
<b>Field added. </b>
<code>u8 is_active</code>
</li>
<li>
<b>Field added. </b>
<code>short unsigned int eoi_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int irq_epoch</code>
</li>
<li>
<b>Field added. </b>
<code>u64 eoi_time</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>int refcnt</code> ➡️ <code>short int refcnt</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum xen_irq_type type</code> ➡️ <code>short int type</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool is_static</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rcu_work rwork</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head *head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>int refcnt</code>
</li>
<li>
<b>Field removed. </b>
<code>enum xen_irq_type type</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int evtchn</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>union (anon) u</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int irq</code> ➡️ <code>int irq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head *head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>int refcnt</code>
</li>
<li>
<b>Field removed. </b>
<code>enum xen_irq_type type</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int evtchn</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>union (anon) u</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int irq</code> ➡️ <code>int irq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head *head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>int refcnt</code>
</li>
<li>
<b>Field removed. </b>
<code>enum xen_irq_type type</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int evtchn</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>union (anon) u</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int irq</code> ➡️ <code>int irq</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head *head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>int refcnt</code>
</li>
<li>
<b>Field removed. </b>
<code>enum xen_irq_type type</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int evtchn</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>union (anon) u</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int irq</code> ➡️ <code>int irq</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

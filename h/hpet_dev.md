# Struct: <code>hpet_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hpet_dev {
    struct clock_event_device evt;
    unsigned int num;
    int cpu;
    unsigned int irq;
    unsigned int flags;
    char name[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
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
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hpet_dev {
    struct hpets *hd_hpets;
    struct hpet *hd_hpet;
    struct hpet_timer *hd_timer;
    long unsigned int hd_ireqfreq;
    long unsigned int hd_irqdata;
    wait_queue_head_t hd_waitqueue;
    struct fasync_struct *hd_async_queue;
    unsigned int hd_flags;
    unsigned int hd_irq;
    unsigned int hd_hdwirq;
    char hd_name[7];
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hpets *hd_hpets</code>
</li>
<li>
<b>Field added. </b>
<code>struct hpet *hd_hpet</code>
</li>
<li>
<b>Field added. </b>
<code>struct hpet_timer *hd_timer</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int hd_ireqfreq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int hd_irqdata</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t hd_waitqueue</code>
</li>
<li>
<b>Field added. </b>
<code>struct fasync_struct *hd_async_queue</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int hd_flags</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int hd_irq</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int hd_hdwirq</code>
</li>
<li>
<b>Field added. </b>
<code>char hd_name[7]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct clock_event_device evt</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int num</code>
</li>
<li>
<b>Field removed. </b>
<code>int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int irq</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
</li>
<li>
<b>Field removed. </b>
<code>char name[10]</code>
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

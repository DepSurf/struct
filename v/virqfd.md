# Struct: <code>virqfd</code>

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
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct virqfd {
    void *opaque;
    struct eventfd_ctx *eventfd;
    int (*handler)(void *, void *);
    void (*thread)(void *, void *);
    void *data;
    struct work_struct inject;
    wait_queue_entry_t wait;
    poll_table pt;
    struct work_struct shutdown;
    struct virqfd **pvirqfd;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
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

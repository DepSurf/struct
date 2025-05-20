# Struct: <code>wwan_port</code>

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
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct wwan_port {
    enum wwan_port_type type;
    unsigned int start_count;
    long unsigned int flags;
    const struct wwan_port_ops *ops;
    struct mutex ops_lock;
    struct device dev;
    struct sk_buff_head rxq;
    wait_queue_head_t waitqueue;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct wwan_port {
    enum wwan_port_type type;
    unsigned int start_count;
    long unsigned int flags;
    const struct wwan_port_ops *ops;
    struct mutex ops_lock;
    struct device dev;
    struct sk_buff_head rxq;
    wait_queue_head_t waitqueue;
    struct mutex data_lock;
    struct (anon) at_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct wwan_port {
    enum wwan_port_type type;
    unsigned int start_count;
    long unsigned int flags;
    const struct wwan_port_ops *ops;
    struct mutex ops_lock;
    struct device dev;
    struct sk_buff_head rxq;
    wait_queue_head_t waitqueue;
    struct mutex data_lock;
    struct (anon) at_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct wwan_port {
    enum wwan_port_type type;
    unsigned int start_count;
    long unsigned int flags;
    const struct wwan_port_ops *ops;
    struct mutex ops_lock;
    struct device dev;
    struct sk_buff_head rxq;
    wait_queue_head_t waitqueue;
    struct mutex data_lock;
    struct (anon) at_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct wwan_port {
    enum wwan_port_type type;
    unsigned int start_count;
    long unsigned int flags;
    const struct wwan_port_ops *ops;
    struct mutex ops_lock;
    struct device dev;
    struct sk_buff_head rxq;
    wait_queue_head_t waitqueue;
    struct mutex data_lock;
    size_t headroom_len;
    size_t frag_len;
    struct (anon) at_data;
};
```
</details>
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
In <code>ppc64el</code>: Absent ⚠️
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
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex data_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) at_data</code>
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
<code>size_t headroom_len</code>
</li>
<li>
<b>Field added. </b>
<code>size_t frag_len</code>
</li>
</ul>
</details>
</li>
</ul>

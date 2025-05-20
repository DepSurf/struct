# Struct: <code>trace_event_raw_xhci_log_ring</code>

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
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int bounce_buf_len;
    char __data[0];
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
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
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
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_event_raw_xhci_log_ring {
    struct trace_entry ent;
    u32 type;
    void *ring;
    dma_addr_t enq;
    dma_addr_t deq;
    dma_addr_t enq_seg;
    dma_addr_t deq_seg;
    unsigned int num_segs;
    unsigned int stream_id;
    unsigned int cycle_state;
    unsigned int num_trbs_free;
    unsigned int bounce_buf_len;
    char __data[0];
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
<b>Field removed. </b>
<code>unsigned int num_trbs_free</code>
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

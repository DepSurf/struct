# Struct: <code>xhci_virt_ep</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_td *stopped_td;
    unsigned int stopped_stream;
    struct timer_list stop_cmd_timer;
    int stop_cmds_pending;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_td *stopped_td;
    unsigned int stopped_stream;
    struct timer_list stop_cmd_timer;
    int stop_cmds_pending;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_td *stopped_td;
    unsigned int stopped_stream;
    struct timer_list stop_cmd_timer;
    int stop_cmds_pending;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_virt_device *vdev;
    unsigned int ep_index;
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_virt_device *vdev;
    unsigned int ep_index;
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_virt_device *vdev;
    unsigned int ep_index;
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_virt_device *vdev;
    unsigned int ep_index;
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int err_count;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_virt_device *vdev;
    unsigned int ep_index;
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int err_count;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_virt_device *vdev;
    unsigned int ep_index;
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int err_count;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
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
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
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
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xhci_virt_ep {
    struct xhci_ring *ring;
    struct xhci_stream_info *stream_info;
    struct xhci_ring *new_ring;
    unsigned int ep_state;
    struct list_head cancelled_td_list;
    struct timer_list stop_cmd_timer;
    struct xhci_hcd *xhci;
    struct xhci_segment *queued_deq_seg;
    union xhci_trb *queued_deq_ptr;
    bool skip;
    struct xhci_bw_info bw_info;
    struct list_head bw_endpoint_list;
    int next_frame_id;
    bool use_extended_tbc;
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
<b>Field removed. </b>
<code>struct xhci_td *stopped_td</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int stopped_stream</code>
</li>
<li>
<b>Field removed. </b>
<code>int stop_cmds_pending</code>
</li>
</ul>
</details>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct xhci_virt_device *vdev</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ep_index</code>
</li>
</ul>
</details>
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
<code>struct timer_list stop_cmd_timer</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int err_count</code>
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

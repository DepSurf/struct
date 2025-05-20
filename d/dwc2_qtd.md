# Struct: <code>dwc2_qtd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
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
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
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
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dwc2_qtd {
    enum dwc2_control_phase control_phase;
    u8 in_process;
    u8 data_toggle;
    u8 complete_split;
    u8 isoc_split_pos;
    u16 isoc_frame_index;
    u16 isoc_split_offset;
    u16 isoc_td_last;
    u16 isoc_td_first;
    u32 ssplit_out_xfer_count;
    u8 error_count;
    u8 n_desc;
    u16 isoc_frame_index_last;
    u16 num_naks;
    struct dwc2_hcd_urb *urb;
    struct dwc2_qh *qh;
    struct list_head qtd_list_entry;
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
<code>u16 isoc_td_last</code>
</li>
<li>
<b>Field added. </b>
<code>u16 isoc_td_first</code>
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 num_naks</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

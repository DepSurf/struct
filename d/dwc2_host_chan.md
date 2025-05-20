# Struct: <code>dwc2_host_chan</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
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
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
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
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
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
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dwc2_host_chan {
    u8 hc_num;
    unsigned int dev_addr;
    unsigned int ep_num;
    unsigned int ep_is_in;
    unsigned int speed;
    unsigned int ep_type;
    unsigned int max_packet;
    unsigned int data_pid_start;
    unsigned int multi_count;
    u8 *xfer_buf;
    dma_addr_t xfer_dma;
    dma_addr_t align_buf;
    u32 xfer_len;
    u32 xfer_count;
    u16 start_pkt_count;
    u8 xfer_started;
    u8 do_ping;
    u8 error_state;
    u8 halt_on_queue;
    u8 halt_pending;
    u8 do_split;
    u8 complete_split;
    u8 hub_addr;
    u8 hub_port;
    u8 xact_pos;
    u8 requests;
    u8 schinfo;
    u16 ntd;
    enum dwc2_halt_status halt_status;
    u32 hcint;
    struct dwc2_qh *qh;
    struct list_head hc_list_entry;
    dma_addr_t desc_list_addr;
    u32 desc_list_sz;
    struct list_head split_order_list_entry;
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
<code>u32 desc_list_sz</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head split_order_list_entry</code>
</li>
<li>
<b>Field removed. </b>
<code>dma_addr_t align_buf</code>
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
<code>dma_addr_t align_buf</code>
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

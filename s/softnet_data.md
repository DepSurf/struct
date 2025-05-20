# Struct: <code>softnet_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int cpu_collision;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct call_single_data csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_head;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    unsigned int input_queue_head;
    struct call_single_data csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    unsigned int input_queue_head;
    struct call_single_data csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    unsigned int input_queue_head;
    struct call_single_data csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
    spinlock_t defer_lock;
    int defer_count;
    int defer_ipi_scheduled;
    struct sk_buff *defer_list;
    call_single_data_t defer_csd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int received_rps;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
    spinlock_t defer_lock;
    int defer_count;
    int defer_ipi_scheduled;
    struct sk_buff *defer_list;
    call_single_data_t defer_csd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    struct softnet_data *rps_ipi_list;
    bool in_net_rx_action;
    bool in_napi_threaded_poll;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int received_rps;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
    spinlock_t defer_lock;
    int defer_count;
    int defer_ipi_scheduled;
    struct sk_buff *defer_list;
    call_single_data_t defer_csd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    struct softnet_data *rps_ipi_list;
    bool in_net_rx_action;
    bool in_napi_threaded_poll;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int received_rps;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
    spinlock_t defer_lock;
    int defer_count;
    int defer_ipi_scheduled;
    struct sk_buff *defer_list;
    call_single_data_t defer_csd;
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
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
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
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct softnet_data {
    struct list_head poll_list;
    struct sk_buff_head process_queue;
    unsigned int processed;
    unsigned int time_squeeze;
    unsigned int received_rps;
    struct softnet_data *rps_ipi_list;
    struct sd_flow_limit *flow_limit;
    struct Qdisc *output_queue;
    struct Qdisc **output_queue_tailp;
    struct sk_buff *completion_queue;
    struct sk_buff_head xfrm_backlog;
    struct (anon) xmit;
    unsigned int input_queue_head;
    call_single_data_t csd;
    struct softnet_data *rps_ipi_next;
    unsigned int cpu;
    unsigned int input_queue_tail;
    unsigned int dropped;
    struct sk_buff_head input_pkt_queue;
    struct napi_struct backlog;
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
<b>Field removed. </b>
<code>unsigned int cpu_collision</code>
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct call_single_data csd</code> ➡️ <code>call_single_data_t csd</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff_head xfrm_backlog</code>
</li>
</ul>
</details>
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
<code>struct (anon) xmit</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t defer_lock</code>
</li>
<li>
<b>Field added. </b>
<code>int defer_count</code>
</li>
<li>
<b>Field added. </b>
<code>int defer_ipi_scheduled</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff *defer_list</code>
</li>
<li>
<b>Field added. </b>
<code>call_single_data_t defer_csd</code>
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
<code>bool in_net_rx_action</code>
</li>
<li>
<b>Field added. </b>
<code>bool in_napi_threaded_poll</code>
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

# Struct: <code>tcp_congestion_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, u32, s32);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*tso_segs_goal)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*tso_segs_goal)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*tso_segs_goal)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    u32 (*undo_cwnd)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    u32 (*undo_cwnd)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    u32 (*undo_cwnd)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    u32 (*undo_cwnd)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    u32 (*undo_cwnd)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    u32 (*undo_cwnd)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
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
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
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
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcp_congestion_ops {
    struct list_head list;
    u32 key;
    u32 flags;
    void (*init)(struct sock *);
    void (*release)(struct sock *);
    u32 (*ssthresh)(struct sock *);
    void (*cong_avoid)(struct sock *, u32, u32);
    void (*set_state)(struct sock *, u8);
    void (*cwnd_event)(struct sock *, enum tcp_ca_event);
    void (*in_ack_event)(struct sock *, u32);
    u32 (*undo_cwnd)(struct sock *);
    void (*pkts_acked)(struct sock *, const struct ack_sample *);
    u32 (*min_tso_segs)(struct sock *);
    u32 (*sndbuf_expand)(struct sock *);
    void (*cong_control)(struct sock *, const struct rate_sample *);
    size_t (*get_info)(struct sock *, u32, int *, union tcp_cc_info *);
    char name[16];
    struct module *owner;
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
<b>Field type changed. </b>
<code>void (*pkts_acked)(struct sock *, u32, s32)</code> ➡️ <code>void (*pkts_acked)(struct sock *, const struct ack_sample *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 (*tso_segs_goal)(struct sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>u32 (*sndbuf_expand)(struct sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*cong_control)(struct sock *, const struct rate_sample *)</code>
</li>
</ul>
</details>
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
<code>u32 (*min_tso_segs)(struct sock *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 (*tso_segs_goal)(struct sock *)</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

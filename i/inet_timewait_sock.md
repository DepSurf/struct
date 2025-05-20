# Struct: <code>inet_timewait_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    int tw_timeout;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    int tw_timeout;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    int tw_timeout;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    int tw_timeout;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    int tw_timeout;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
    struct inet_bind2_bucket *tw_tb2;
    struct hlist_node tw_bind2_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
    struct inet_bind2_bucket *tw_tb2;
    struct hlist_node tw_bind2_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_usec_ts;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
    struct inet_bind2_bucket *tw_tb2;
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
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
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
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_timewait_sock {
    struct sock_common __tw_common;
    __u32 tw_mark;
    volatile unsigned char tw_substate;
    unsigned char tw_rcv_wscale;
    __be16 tw_sport;
    unsigned int tw_kill;
    unsigned int tw_transparent;
    unsigned int tw_flowlabel;
    unsigned int tw_pad;
    unsigned int tw_tos;
    u32 tw_txhash;
    u32 tw_priority;
    struct timer_list tw_timer;
    struct inet_bind_bucket *tw_tb;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 tw_mark</code>
</li>
<li>
<b>Field removed. </b>
<code>int tw_timeout</code>
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
<code>u32 tw_txhash</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 tw_priority</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>unsigned int tw_kill</code>
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
<code>struct inet_bind2_bucket *tw_tb2</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node tw_bind2_node</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int tw_usec_ts</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node tw_bind2_node</code>
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

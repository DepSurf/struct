# Struct: <code>bpf_sock_ops_kern</code>

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
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 reply;
    u32 replylong[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 reply;
    u32 replylong[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    struct sk_buff *syn_skb;
    struct sk_buff *skb;
    void *skb_data_end;
    u8 op;
    u8 is_fullsock;
    u8 remaining_opt_len;
    u64 temp;
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
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
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
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_sock_ops_kern {
    struct sock *sk;
    u32 op;
    u32 args[4];
    u32 reply;
    u32 replylong[4];
    u32 is_fullsock;
    u64 temp;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 args[4]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 is_fullsock</code>
</li>
<li>
<b>Field added. </b>
<code>u64 temp</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff *syn_skb</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff *skb</code>
</li>
<li>
<b>Field added. </b>
<code>void *skb_data_end</code>
</li>
<li>
<b>Field added. </b>
<code>u8 remaining_opt_len</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 op</code> ➡️ <code>u8 op</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 is_fullsock</code> ➡️ <code>u8 is_fullsock</code>
</li>
</ul>
</details>
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

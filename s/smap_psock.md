# Struct: <code>smap_psock</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct smap_psock {
    struct callback_head rcu;
    u32 refcnt;
    struct sk_buff_head rxqueue;
    bool strp_enabled;
    int save_rem;
    int save_off;
    struct sk_buff *save_skb;
    struct strparser strp;
    struct bpf_prog *bpf_parse;
    struct bpf_prog *bpf_verdict;
    struct list_head maps;
    struct sock *sock;
    long unsigned int state;
    struct work_struct tx_work;
    struct work_struct gc_work;
    void (*save_data_ready)(struct sock *);
    void (*save_write_space)(struct sock *);
    void (*save_state_change)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct smap_psock {
    struct callback_head rcu;
    refcount_t refcnt;
    struct sk_buff_head rxqueue;
    bool strp_enabled;
    int save_rem;
    int save_off;
    struct sk_buff *save_skb;
    struct sock *sk_redir;
    int apply_bytes;
    int cork_bytes;
    int sg_size;
    int eval;
    struct sk_msg_buff *cork;
    struct list_head ingress;
    struct strparser strp;
    struct bpf_prog *bpf_tx_msg;
    struct bpf_prog *bpf_parse;
    struct bpf_prog *bpf_verdict;
    struct list_head maps;
    spinlock_t maps_lock;
    struct sock *sock;
    long unsigned int state;
    struct work_struct tx_work;
    struct work_struct gc_work;
    struct proto *sk_proto;
    void (*save_close)(struct sock *, long int);
    void (*save_data_ready)(struct sock *);
    void (*save_write_space)(struct sock *);
};
```
</details>
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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sock *sk_redir</code>
</li>
<li>
<b>Field added. </b>
<code>int apply_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>int cork_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>int sg_size</code>
</li>
<li>
<b>Field added. </b>
<code>int eval</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_msg_buff *cork</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head ingress</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_prog *bpf_tx_msg</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t maps_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct proto *sk_proto</code>
</li>
<li>
<b>Field added. </b>
<code>void (*save_close)(struct sock *, long int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*save_state_change)(struct sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 refcnt</code> ➡️ <code>refcount_t refcnt</code>
</li>
</ul>
</details>
</li>
</ul>

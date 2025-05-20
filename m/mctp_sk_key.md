# Struct: <code>mctp_sk_key</code>

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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mctp_sk_key {
    mctp_eid_t peer_addr;
    mctp_eid_t local_addr;
    __u8 tag;
    struct sock *sk;
    struct hlist_node hlist;
    struct hlist_node sklist;
    spinlock_t lock;
    refcount_t refs;
    struct sk_buff *reasm_head;
    struct sk_buff **reasm_tailp;
    bool reasm_dead;
    u8 last_seq;
    bool valid;
    long unsigned int expiry;
    long unsigned int dev_flow_state;
    struct mctp_dev *dev;
    bool manual_alloc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mctp_sk_key {
    mctp_eid_t peer_addr;
    mctp_eid_t local_addr;
    __u8 tag;
    struct sock *sk;
    struct hlist_node hlist;
    struct hlist_node sklist;
    spinlock_t lock;
    refcount_t refs;
    struct sk_buff *reasm_head;
    struct sk_buff **reasm_tailp;
    bool reasm_dead;
    u8 last_seq;
    bool valid;
    long unsigned int expiry;
    long unsigned int dev_flow_state;
    struct mctp_dev *dev;
    bool manual_alloc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mctp_sk_key {
    mctp_eid_t peer_addr;
    mctp_eid_t local_addr;
    __u8 tag;
    struct sock *sk;
    struct hlist_node hlist;
    struct hlist_node sklist;
    spinlock_t lock;
    refcount_t refs;
    struct sk_buff *reasm_head;
    struct sk_buff **reasm_tailp;
    bool reasm_dead;
    u8 last_seq;
    bool valid;
    long unsigned int expiry;
    long unsigned int dev_flow_state;
    struct mctp_dev *dev;
    bool manual_alloc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mctp_sk_key {
    mctp_eid_t peer_addr;
    mctp_eid_t local_addr;
    __u8 tag;
    struct sock *sk;
    struct hlist_node hlist;
    struct hlist_node sklist;
    spinlock_t lock;
    refcount_t refs;
    struct sk_buff *reasm_head;
    struct sk_buff **reasm_tailp;
    bool reasm_dead;
    u8 last_seq;
    bool valid;
    long unsigned int expiry;
    long unsigned int dev_flow_state;
    struct mctp_dev *dev;
    bool manual_alloc;
};
```
</details>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

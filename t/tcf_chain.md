# Struct: <code>tcf_chain</code>

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
struct tcf_chain {
    struct tcf_proto *filter_chain;
    struct tcf_proto **p_filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcf_chain {
    struct tcf_proto *filter_chain;
    tcf_chain_head_change_t *chain_head_change;
    void *chain_head_change_priv;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcf_chain {
    struct tcf_proto *filter_chain;
    struct list_head filter_chain_list;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcf_chain {
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
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
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
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
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcf_chain {
    struct mutex filter_chain_lock;
    struct tcf_proto *filter_chain;
    struct list_head list;
    struct tcf_block *block;
    u32 index;
    unsigned int refcnt;
    unsigned int action_refcnt;
    bool explicitly_created;
    bool flushing;
    const struct tcf_proto_ops *tmplt_ops;
    void *tmplt_priv;
    struct callback_head rcu;
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>tcf_chain_head_change_t *chain_head_change</code>
</li>
<li>
<b>Field added. </b>
<code>void *chain_head_change_priv</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tcf_proto **p_filter_chain</code>
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
<code>struct list_head filter_chain_list</code>
</li>
<li>
<b>Field removed. </b>
<code>tcf_chain_head_change_t *chain_head_change</code>
</li>
<li>
<b>Field removed. </b>
<code>void *chain_head_change_priv</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int action_refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>bool explicitly_created</code>
</li>
<li>
<b>Field added. </b>
<code>const struct tcf_proto_ops *tmplt_ops</code>
</li>
<li>
<b>Field added. </b>
<code>void *tmplt_priv</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head filter_chain_list</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex filter_chain_lock</code>
</li>
<li>
<b>Field added. </b>
<code>bool flushing</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
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

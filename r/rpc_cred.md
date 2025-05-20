# Struct: <code>rpc_cred</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_magic;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    atomic_t cr_count;
    kuid_t cr_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_magic;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    atomic_t cr_count;
    kuid_t cr_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    atomic_t cr_count;
    kuid_t cr_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    atomic_t cr_count;
    kuid_t cr_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    atomic_t cr_count;
    kuid_t cr_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
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
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
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
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rpc_cred {
    struct hlist_node cr_hash;
    struct list_head cr_lru;
    struct callback_head cr_rcu;
    struct rpc_auth *cr_auth;
    const struct rpc_credops *cr_ops;
    long unsigned int cr_expire;
    long unsigned int cr_flags;
    refcount_t cr_count;
    const struct cred *cr_cred;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int cr_magic</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct cred *cr_cred</code>
</li>
<li>
<b>Field removed. </b>
<code>kuid_t cr_uid</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t cr_count</code> ➡️ <code>refcount_t cr_count</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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

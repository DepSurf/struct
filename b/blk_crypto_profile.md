# Struct: <code>blk_crypto_profile</code>

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
struct blk_crypto_profile {
    struct blk_crypto_ll_ops ll_ops;
    unsigned int max_dun_bytes_supported;
    unsigned int modes_supported[4];
    struct device *dev;
    unsigned int num_slots;
    struct rw_semaphore lock;
    wait_queue_head_t idle_slots_wait_queue;
    struct list_head idle_slots;
    spinlock_t idle_slots_lock;
    struct hlist_head *slot_hashtable;
    unsigned int log_slot_ht_size;
    struct blk_crypto_keyslot *slots;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blk_crypto_profile {
    struct blk_crypto_ll_ops ll_ops;
    unsigned int max_dun_bytes_supported;
    unsigned int modes_supported[5];
    struct device *dev;
    unsigned int num_slots;
    struct rw_semaphore lock;
    wait_queue_head_t idle_slots_wait_queue;
    struct list_head idle_slots;
    spinlock_t idle_slots_lock;
    struct hlist_head *slot_hashtable;
    unsigned int log_slot_ht_size;
    struct blk_crypto_keyslot *slots;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blk_crypto_profile {
    struct blk_crypto_ll_ops ll_ops;
    unsigned int max_dun_bytes_supported;
    unsigned int modes_supported[5];
    struct device *dev;
    unsigned int num_slots;
    struct rw_semaphore lock;
    struct lock_class_key lockdep_key;
    wait_queue_head_t idle_slots_wait_queue;
    struct list_head idle_slots;
    spinlock_t idle_slots_lock;
    struct hlist_head *slot_hashtable;
    unsigned int log_slot_ht_size;
    struct blk_crypto_keyslot *slots;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blk_crypto_profile {
    struct blk_crypto_ll_ops ll_ops;
    unsigned int max_dun_bytes_supported;
    unsigned int modes_supported[5];
    struct device *dev;
    unsigned int num_slots;
    struct rw_semaphore lock;
    struct lock_class_key lockdep_key;
    wait_queue_head_t idle_slots_wait_queue;
    struct list_head idle_slots;
    spinlock_t idle_slots_lock;
    struct hlist_head *slot_hashtable;
    unsigned int log_slot_ht_size;
    struct blk_crypto_keyslot *slots;
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int modes_supported[4]</code> ➡️ <code>unsigned int modes_supported[5]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct lock_class_key lockdep_key</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

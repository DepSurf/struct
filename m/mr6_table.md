# Struct: <code>mr6_table</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mr6_table {
    struct list_head list;
    possible_net_t net;
    u32 id;
    struct sock *mroute6_sk;
    struct timer_list ipmr_expire_timer;
    struct list_head mfc6_unres_queue;
    struct list_head mfc6_cache_array[64];
    struct mif_device vif6_table[32];
    int maxvif;
    atomic_t cache_resolve_queue_len;
    bool mroute_do_assert;
    bool mroute_do_pim;
    int mroute_reg_vif_num;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mr6_table {
    struct list_head list;
    possible_net_t net;
    u32 id;
    struct sock *mroute6_sk;
    struct timer_list ipmr_expire_timer;
    struct list_head mfc6_unres_queue;
    struct list_head mfc6_cache_array[64];
    struct mif_device vif6_table[32];
    int maxvif;
    atomic_t cache_resolve_queue_len;
    bool mroute_do_assert;
    bool mroute_do_pim;
    int mroute_reg_vif_num;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mr6_table {
    struct list_head list;
    possible_net_t net;
    u32 id;
    struct sock *mroute6_sk;
    struct timer_list ipmr_expire_timer;
    struct list_head mfc6_unres_queue;
    struct list_head mfc6_cache_array[64];
    struct mif_device vif6_table[32];
    int maxvif;
    atomic_t cache_resolve_queue_len;
    bool mroute_do_assert;
    bool mroute_do_pim;
    int mroute_reg_vif_num;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mr6_table {
    struct list_head list;
    possible_net_t net;
    u32 id;
    struct sock *mroute6_sk;
    struct timer_list ipmr_expire_timer;
    struct list_head mfc6_unres_queue;
    struct list_head mfc6_cache_array[64];
    struct mif_device vif6_table[32];
    int maxvif;
    atomic_t cache_resolve_queue_len;
    bool mroute_do_assert;
    bool mroute_do_pim;
    int mroute_reg_vif_num;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mr6_table {
    struct list_head list;
    possible_net_t net;
    u32 id;
    struct sock *mroute6_sk;
    struct timer_list ipmr_expire_timer;
    struct list_head mfc6_unres_queue;
    struct list_head mfc6_cache_array[64];
    struct mif_device vif6_table[32];
    int maxvif;
    atomic_t cache_resolve_queue_len;
    bool mroute_do_assert;
    bool mroute_do_pim;
    int mroute_reg_vif_num;
};
```
</details>
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
</ul>

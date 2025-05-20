# Struct: <code>neigh_parms</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    atomic_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    atomic_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    atomic_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    void (*neigh_cleanup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    u32 qlen;
    int data[14];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    u32 qlen;
    int data[14];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    u32 qlen;
    int data[14];
    long unsigned int data_state[1];
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
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
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
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct neigh_parms {
    possible_net_t net;
    struct net_device *dev;
    struct list_head list;
    int (*neigh_setup)(struct neighbour *);
    struct neigh_table *tbl;
    void *sysctl_table;
    int dead;
    refcount_t refcnt;
    struct callback_head callback_head;
    int reachable_time;
    int data[13];
    long unsigned int data_state[1];
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t refcnt</code> ➡️ <code>refcount_t refcnt</code>
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*neigh_cleanup)(struct neighbour *)</code>
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
<b>Field added. </b>
<code>netdevice_tracker dev_tracker</code>
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
<code>u32 qlen</code>
</li>
<li>
<b>Field type changed. </b>
<code>int data[13]</code> ➡️ <code>int data[14]</code>
</li>
</ul>
</details>
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

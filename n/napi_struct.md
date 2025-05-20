# Struct: <code>napi_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    unsigned int gro_count;
    int (*poll)(struct napi_struct *, int);
    spinlock_t poll_lock;
    int poll_owner;
    struct net_device *dev;
    struct sk_buff *gro_list;
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    unsigned int gro_count;
    int (*poll)(struct napi_struct *, int);
    spinlock_t poll_lock;
    int poll_owner;
    struct net_device *dev;
    struct sk_buff *gro_list;
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    unsigned int gro_count;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct sk_buff *gro_list;
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    unsigned int gro_count;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct sk_buff *gro_list;
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    unsigned int gro_count;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct sk_buff *gro_list;
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    unsigned int gro_count;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct sk_buff *gro_list;
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
    struct task_struct *thread;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
    struct task_struct *thread;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
    struct task_struct *thread;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
    struct task_struct *thread;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    int list_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    unsigned int napi_id;
    struct hrtimer timer;
    struct task_struct *thread;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    int defer_hard_irqs_count;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    int list_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    unsigned int napi_id;
    struct hrtimer timer;
    struct task_struct *thread;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    int irq;
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
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
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
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct napi_struct {
    struct list_head poll_list;
    long unsigned int state;
    int weight;
    long unsigned int gro_bitmask;
    int (*poll)(struct napi_struct *, int);
    int poll_owner;
    struct net_device *dev;
    struct gro_list gro_hash[8];
    struct sk_buff *skb;
    struct list_head rx_list;
    int rx_count;
    struct hrtimer timer;
    struct list_head dev_list;
    struct hlist_node napi_hash_node;
    unsigned int napi_id;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t poll_lock</code>
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int gro_bitmask</code>
</li>
<li>
<b>Field added. </b>
<code>struct gro_list gro_hash[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int gro_count</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff *gro_list</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head rx_list</code>
</li>
<li>
<b>Field added. </b>
<code>int rx_count</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int defer_hard_irqs_count</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct task_struct *thread</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int list_owner</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int irq</code>
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

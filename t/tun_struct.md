# Struct: <code>tun_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    struct tun_pcpu_stats *pcpu_stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    struct tun_pcpu_stats *pcpu_stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
    struct file *file;
    struct ifreq *ifr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
    struct file *file;
    struct ifreq *ifr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
    struct file *file;
    struct ifreq *ifr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
    struct file *file;
    struct ifreq *ifr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    u32 msg_enable;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    atomic_long_t rx_frame_errors;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
    struct file *file;
    struct ifreq *ifr;
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
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
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
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tun_struct {
    struct tun_file * tfiles[256];
    unsigned int numqueues;
    unsigned int flags;
    kuid_t owner;
    kgid_t group;
    struct net_device *dev;
    netdev_features_t set_features;
    int align;
    int vnet_hdr_sz;
    int sndbuf;
    struct tap_filter txflt;
    struct sock_fprog fprog;
    bool filter_attached;
    spinlock_t lock;
    struct hlist_head flows[1024];
    struct timer_list flow_gc_timer;
    long unsigned int ageing_time;
    unsigned int numdisabled;
    struct list_head disabled;
    void *security;
    u32 flow_count;
    u32 rx_batched;
    struct tun_pcpu_stats *pcpu_stats;
    struct bpf_prog *xdp_prog;
    struct tun_prog *steering_prog;
    struct tun_prog *filter_prog;
    struct ethtool_link_ksettings link_ksettings;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int align</code>
</li>
<li>
<b>Field added. </b>
<code>struct tun_pcpu_stats *pcpu_stats</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 rx_batched</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_prog *xdp_prog</code>
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
<code>struct tun_prog *steering_prog</code>
</li>
<li>
<b>Field added. </b>
<code>struct tun_prog *filter_prog</code>
</li>
<li>
<b>Field added. </b>
<code>struct ethtool_link_ksettings link_ksettings</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 msg_enable</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_long_t rx_frame_errors</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tun_pcpu_stats *pcpu_stats</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct file *file</code>
</li>
<li>
<b>Field added. </b>
<code>struct ifreq *ifr</code>
</li>
</ul>
</details>
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

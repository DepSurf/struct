# Struct: <code>virtnet_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct virtnet_info {
    struct virtio_device *vdev;
    struct virtqueue *cvq;
    struct net_device *dev;
    struct send_queue *sq;
    struct receive_queue *rq;
    unsigned int status;
    u16 max_queue_pairs;
    u16 curr_queue_pairs;
    bool big_packets;
    bool mergeable_rx_bufs;
    bool has_cvq;
    bool any_header_sg;
    u8 hdr_len;
    struct virtnet_stats *stats;
    struct delayed_work refill;
    struct work_struct config_work;
    bool affinity_hint_set;
    struct notifier_block nb;
    struct virtio_net_ctrl_hdr ctrl_hdr;
    virtio_net_ctrl_ack ctrl_status;
    u8 ctrl_promisc;
    u8 ctrl_allmulti;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct virtnet_info {
    struct virtio_device *vdev;
    struct virtqueue *cvq;
    struct net_device *dev;
    struct send_queue *sq;
    struct receive_queue *rq;
    unsigned int status;
    u16 max_queue_pairs;
    u16 curr_queue_pairs;
    bool big_packets;
    bool mergeable_rx_bufs;
    bool has_cvq;
    bool any_header_sg;
    u8 hdr_len;
    struct virtnet_stats *stats;
    struct delayed_work refill;
    struct work_struct config_work;
    bool affinity_hint_set;
    struct notifier_block nb;
    struct virtio_net_ctrl_hdr ctrl_hdr;
    virtio_net_ctrl_ack ctrl_status;
    struct virtio_net_ctrl_mq ctrl_mq;
    u8 ctrl_promisc;
    u8 ctrl_allmulti;
    u16 ctrl_vid;
    u8 duplex;
    u32 speed;
};
```
</details>
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
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct virtnet_info {
    struct virtio_device *vdev;
    struct virtqueue *cvq;
    struct net_device *dev;
    struct send_queue *sq;
    struct receive_queue *rq;
    unsigned int status;
    u16 max_queue_pairs;
    u16 curr_queue_pairs;
    u16 xdp_queue_pairs;
    bool xdp_enabled;
    bool big_packets;
    unsigned int big_packets_num_skbfrags;
    bool mergeable_rx_bufs;
    bool has_rss;
    bool has_rss_hash_report;
    u8 rss_key_size;
    u16 rss_indir_table_size;
    u32 rss_hash_types_supported;
    u32 rss_hash_types_saved;
    bool has_cvq;
    bool any_header_sg;
    u8 hdr_len;
    struct delayed_work refill;
    bool refill_enabled;
    spinlock_t refill_lock;
    struct work_struct config_work;
    bool affinity_hint_set;
    struct hlist_node node;
    struct hlist_node node_dead;
    struct control_buf *ctrl;
    u8 duplex;
    u32 speed;
    u32 tx_usecs;
    u32 rx_usecs;
    u32 tx_max_packets;
    u32 rx_max_packets;
    long unsigned int guest_offloads;
    long unsigned int guest_offloads_capable;
    struct failover *failover;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtnet_info {
    struct virtio_device *vdev;
    struct virtqueue *cvq;
    struct net_device *dev;
    struct send_queue *sq;
    struct receive_queue *rq;
    unsigned int status;
    u16 max_queue_pairs;
    u16 curr_queue_pairs;
    u16 xdp_queue_pairs;
    bool xdp_enabled;
    bool big_packets;
    unsigned int big_packets_num_skbfrags;
    bool mergeable_rx_bufs;
    bool has_rss;
    bool has_rss_hash_report;
    u8 rss_key_size;
    u16 rss_indir_table_size;
    u32 rss_hash_types_supported;
    u32 rss_hash_types_saved;
    bool has_cvq;
    bool any_header_sg;
    u8 hdr_len;
    struct delayed_work refill;
    bool refill_enabled;
    spinlock_t refill_lock;
    struct work_struct config_work;
    bool affinity_hint_set;
    struct hlist_node node;
    struct hlist_node node_dead;
    struct control_buf *ctrl;
    u8 duplex;
    u32 speed;
    bool rx_dim_enabled;
    struct virtnet_interrupt_coalesce intr_coal_tx;
    struct virtnet_interrupt_coalesce intr_coal_rx;
    long unsigned int guest_offloads;
    long unsigned int guest_offloads_capable;
    struct failover *failover;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct virtio_net_ctrl_mq ctrl_mq</code>
</li>
<li>
<b>Field added. </b>
<code>u16 ctrl_vid</code>
</li>
<li>
<b>Field added. </b>
<code>u8 duplex</code>
</li>
<li>
<b>Field added. </b>
<code>u32 speed</code>
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
<code>bool rx_dim_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>struct virtnet_interrupt_coalesce intr_coal_tx</code>
</li>
<li>
<b>Field added. </b>
<code>struct virtnet_interrupt_coalesce intr_coal_rx</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 tx_usecs</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rx_usecs</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 tx_max_packets</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rx_max_packets</code>
</li>
</ul>
</details>
</li>
</ul>

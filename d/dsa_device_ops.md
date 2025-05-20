# Struct: <code>dsa_device_ops</code>

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
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    unsigned int overhead;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_master;
    bool tail_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_master;
    bool tail_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    unsigned int needed_headroom;
    unsigned int needed_tailroom;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_master;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    int (*connect)(struct dsa_switch *);
    void (*disconnect)(struct dsa_switch *);
    unsigned int needed_headroom;
    unsigned int needed_tailroom;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_master;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    int (*connect)(struct dsa_switch *);
    void (*disconnect)(struct dsa_switch *);
    unsigned int needed_headroom;
    unsigned int needed_tailroom;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_master;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    int (*connect)(struct dsa_switch *);
    void (*disconnect)(struct dsa_switch *);
    unsigned int needed_headroom;
    unsigned int needed_tailroom;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_master;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *);
    void (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    int (*connect)(struct dsa_switch *);
    void (*disconnect)(struct dsa_switch *);
    unsigned int needed_headroom;
    unsigned int needed_tailroom;
    const char *name;
    enum dsa_tag_protocol proto;
    bool promisc_on_conduit;
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
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
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
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dsa_device_ops {
    struct sk_buff * (*xmit)(struct sk_buff *, struct net_device *);
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *);
    int (*flow_dissect)(const struct sk_buff *, __be16 *, int *);
    bool (*filter)(const struct sk_buff *, struct net_device *);
    unsigned int overhead;
    const char *name;
    enum dsa_tag_protocol proto;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int overhead</code>
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
<code>bool (*filter)(const struct sk_buff *, struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>const char *name</code>
</li>
<li>
<b>Field added. </b>
<code>enum dsa_tag_protocol proto</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool promisc_on_master</code>
</li>
<li>
<b>Field added. </b>
<code>bool tail_tag</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*flow_dissect)(const struct sk_buff *, __be16 *, int *)</code> ➡️ <code>void (*flow_dissect)(const struct sk_buff *, __be16 *, int *)</code>
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
<code>unsigned int needed_headroom</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int needed_tailroom</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*filter)(const struct sk_buff *, struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int overhead</code>
</li>
<li>
<b>Field removed. </b>
<code>bool tail_tag</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *)</code> ➡️ <code>struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*connect)(struct dsa_switch *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*disconnect)(struct dsa_switch *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool promisc_on_conduit</code>
</li>
<li>
<b>Field removed. </b>
<code>bool promisc_on_master</code>
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

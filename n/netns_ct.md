# Struct: <code>netns_ct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    struct ctl_table_header *sysctl_header;
    struct ctl_table_header *acct_sysctl_header;
    struct ctl_table_header *tstamp_sysctl_header;
    struct ctl_table_header *event_sysctl_header;
    struct ctl_table_header *helper_sysctl_header;
    char *slabname;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    bool auto_assign_helper_warned;
    int sysctl_tstamp;
    int sysctl_checksum;
    unsigned int htable_size;
    seqcount_t generation;
    struct kmem_cache *nf_conntrack_cachep;
    struct hlist_nulls_head *hash;
    struct hlist_head *expect_hash;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
    u8 label_words;
    struct hlist_head *nat_bysource;
    unsigned int nat_htable_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    struct ctl_table_header *sysctl_header;
    struct ctl_table_header *acct_sysctl_header;
    struct ctl_table_header *tstamp_sysctl_header;
    struct ctl_table_header *event_sysctl_header;
    struct ctl_table_header *helper_sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    bool auto_assign_helper_warned;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
    u8 label_words;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    struct ctl_table_header *sysctl_header;
    struct ctl_table_header *acct_sysctl_header;
    struct ctl_table_header *tstamp_sysctl_header;
    struct ctl_table_header *event_sysctl_header;
    struct ctl_table_header *helper_sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    bool auto_assign_helper_warned;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    struct ctl_table_header *sysctl_header;
    struct ctl_table_header *acct_sysctl_header;
    struct ctl_table_header *tstamp_sysctl_header;
    struct ctl_table_header *event_sysctl_header;
    struct ctl_table_header *helper_sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    bool auto_assign_helper_warned;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    struct ctl_table_header *sysctl_header;
    struct ctl_table_header *acct_sysctl_header;
    struct ctl_table_header *tstamp_sysctl_header;
    struct ctl_table_header *event_sysctl_header;
    struct ctl_table_header *helper_sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    bool auto_assign_helper_warned;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    struct ctl_table_header *sysctl_header;
    struct ctl_table_header *acct_sysctl_header;
    struct ctl_table_header *tstamp_sysctl_header;
    struct ctl_table_header *event_sysctl_header;
    struct ctl_table_header *helper_sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    bool auto_assign_helper_warned;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_ct {
    bool ecache_dwork_pending;
    u8 sysctl_log_invalid;
    u8 sysctl_events;
    u8 sysctl_acct;
    u8 sysctl_auto_assign_helper;
    u8 sysctl_tstamp;
    u8 sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_ct {
    bool ecache_dwork_pending;
    u8 sysctl_log_invalid;
    u8 sysctl_events;
    u8 sysctl_acct;
    u8 sysctl_auto_assign_helper;
    u8 sysctl_tstamp;
    u8 sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_ct {
    u8 ctnetlink_has_listener;
    bool ecache_dwork_pending;
    u8 sysctl_log_invalid;
    u8 sysctl_events;
    u8 sysctl_acct;
    u8 sysctl_auto_assign_helper;
    u8 sysctl_tstamp;
    u8 sysctl_checksum;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_ct {
    bool ecache_dwork_pending;
    u8 sysctl_log_invalid;
    u8 sysctl_events;
    u8 sysctl_acct;
    u8 sysctl_tstamp;
    u8 sysctl_checksum;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_ct {
    bool ecache_dwork_pending;
    u8 sysctl_log_invalid;
    u8 sysctl_events;
    u8 sysctl_acct;
    u8 sysctl_tstamp;
    u8 sysctl_checksum;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_ct {
    bool ecache_dwork_pending;
    u8 sysctl_log_invalid;
    u8 sysctl_events;
    u8 sysctl_acct;
    u8 sysctl_tstamp;
    u8 sysctl_checksum;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_ip_net nf_ct_proto;
    atomic_t labels_used;
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
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
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
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_ct {
    atomic_t count;
    unsigned int expect_count;
    struct delayed_work ecache_dwork;
    bool ecache_dwork_pending;
    bool auto_assign_helper_warned;
    struct ctl_table_header *sysctl_header;
    unsigned int sysctl_log_invalid;
    int sysctl_events;
    int sysctl_acct;
    int sysctl_auto_assign_helper;
    int sysctl_tstamp;
    int sysctl_checksum;
    struct ct_pcpu *pcpu_lists;
    struct ip_conntrack_stat *stat;
    struct nf_ct_event_notifier *nf_conntrack_event_cb;
    struct nf_exp_event_notifier *nf_expect_event_cb;
    struct nf_ip_net nf_ct_proto;
    unsigned int labels_used;
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
<b>Field removed. </b>
<code>char *slabname</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int htable_size</code>
</li>
<li>
<b>Field removed. </b>
<code>seqcount_t generation</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kmem_cache *nf_conntrack_cachep</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_nulls_head *hash</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_head *expect_hash</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_head *nat_bysource</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nat_htable_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 label_words</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ip_conntrack_stat *stat</code> ➡️ <code>struct ip_conntrack_stat *stat</code>
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
<b>Field removed. </b>
<code>struct ctl_table_header *acct_sysctl_header</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ctl_table_header *tstamp_sysctl_header</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ctl_table_header *event_sysctl_header</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ctl_table_header *helper_sysctl_header</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct nf_ct_event_notifier *nf_conntrack_event_cb</code> ➡️ <code>struct nf_ct_event_notifier *nf_conntrack_event_cb</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct nf_exp_event_notifier *nf_expect_event_cb</code> ➡️ <code>struct nf_exp_event_notifier *nf_expect_event_cb</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t count</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int expect_count</code>
</li>
<li>
<b>Field removed. </b>
<code>struct delayed_work ecache_dwork</code>
</li>
<li>
<b>Field removed. </b>
<code>bool auto_assign_helper_warned</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ctl_table_header *sysctl_header</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sysctl_log_invalid</code> ➡️ <code>u8 sysctl_log_invalid</code>
</li>
<li>
<b>Field type changed. </b>
<code>int sysctl_events</code> ➡️ <code>u8 sysctl_events</code>
</li>
<li>
<b>Field type changed. </b>
<code>int sysctl_acct</code> ➡️ <code>u8 sysctl_acct</code>
</li>
<li>
<b>Field type changed. </b>
<code>int sysctl_auto_assign_helper</code> ➡️ <code>u8 sysctl_auto_assign_helper</code>
</li>
<li>
<b>Field type changed. </b>
<code>int sysctl_tstamp</code> ➡️ <code>u8 sysctl_tstamp</code>
</li>
<li>
<b>Field type changed. </b>
<code>int sysctl_checksum</code> ➡️ <code>u8 sysctl_checksum</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct nf_exp_event_notifier *nf_expect_event_cb</code>
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
<code>u8 ctnetlink_has_listener</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ct_pcpu *pcpu_lists</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 ctnetlink_has_listener</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 sysctl_auto_assign_helper</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int labels_used</code> ➡️ <code>atomic_t labels_used</code>
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

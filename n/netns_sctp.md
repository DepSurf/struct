# Struct: <code>netns_sctp</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int auth_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int auth_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int auth_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    unsigned int probe_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    unsigned int probe_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    unsigned int probe_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
    int l3mdev_accept;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    unsigned int probe_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
    int l3mdev_accept;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct sock *udp4_sock;
    struct sock *udp6_sock;
    int udp_port;
    int encap_port;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    unsigned int probe_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int ps_retrans;
    int pf_enable;
    int pf_expose;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
    int l3mdev_accept;
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
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
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
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_sctp {
    struct sctp_mib *sctp_statistics;
    struct proc_dir_entry *proc_net_sctp;
    struct ctl_table_header *sysctl_header;
    struct sock *ctl_sock;
    struct list_head local_addr_list;
    struct list_head addr_waitq;
    struct timer_list addr_wq_timer;
    struct list_head auto_asconf_splist;
    spinlock_t addr_wq_lock;
    spinlock_t local_addr_lock;
    unsigned int rto_initial;
    unsigned int rto_min;
    unsigned int rto_max;
    int rto_alpha;
    int rto_beta;
    int max_burst;
    int cookie_preserve_enable;
    char *sctp_hmac_alg;
    unsigned int valid_cookie_life;
    unsigned int sack_timeout;
    unsigned int hb_interval;
    int max_retrans_association;
    int max_retrans_path;
    int max_retrans_init;
    int pf_retrans;
    int pf_enable;
    int sndbuf_policy;
    int rcvbuf_policy;
    int default_auto_asconf;
    int addip_enable;
    int addip_noauth;
    int prsctp_enable;
    int reconf_enable;
    int auth_enable;
    int intl_enable;
    int ecn_enable;
    int scope_policy;
    int rwnd_upd_shift;
    long unsigned int max_autoclose;
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
<code>int pf_enable</code>
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
<code>int reconf_enable</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int intl_enable</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int ecn_enable</code>
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
<code>int ps_retrans</code>
</li>
<li>
<b>Field added. </b>
<code>int pf_expose</code>
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
<code>struct sock *udp4_sock</code>
</li>
<li>
<b>Field added. </b>
<code>struct sock *udp6_sock</code>
</li>
<li>
<b>Field added. </b>
<code>int udp_port</code>
</li>
<li>
<b>Field added. </b>
<code>int encap_port</code>
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
<code>unsigned int probe_interval</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int l3mdev_accept</code>
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
<details>
<summary>Changed between <code>generic</code> and <code>gcp</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct sctp_mib *sctp_statistics</code> ➡️ <code>struct sctp_mib *sctp_statistics</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

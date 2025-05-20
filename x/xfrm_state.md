# Struct: <code>xfrm_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    atomic_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    long int saved_tmo;
    long unsigned int lastused;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    atomic_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    long int saved_tmo;
    long unsigned int lastused;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    atomic_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    long int saved_tmo;
    long unsigned int lastused;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    long unsigned int lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    long unsigned int lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    long unsigned int lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct tasklet_hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode *inner_mode;
    struct xfrm_mode *inner_mode_iaf;
    struct xfrm_mode *outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    struct hlist_node byseq;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    __be16 new_mapping_sport;
    u32 new_mapping;
    u32 mapping_maxage;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    enum xfrm_replay_mode repl_mode;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    struct hlist_node byseq;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    __be16 new_mapping_sport;
    u32 new_mapping;
    u32 mapping_maxage;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    enum xfrm_replay_mode repl_mode;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_dev_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    struct hlist_node byseq;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    __be16 new_mapping_sport;
    u32 new_mapping;
    u32 mapping_maxage;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    enum xfrm_replay_mode repl_mode;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_dev_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    struct hlist_node byseq;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    __be16 new_mapping_sport;
    u32 new_mapping;
    u32 mapping_maxage;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    enum xfrm_replay_mode repl_mode;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_dev_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    struct hlist_node byseq;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    __be16 new_mapping_sport;
    u32 new_mapping;
    u32 mapping_maxage;
    struct xfrm_encap_tmpl *encap;
    struct sock *encap_sk;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    enum xfrm_replay_mode repl_mode;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_dev_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
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
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
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
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_state {
    possible_net_t xs_net;
    struct hlist_node gclist;
    struct hlist_node bydst;
    struct hlist_node bysrc;
    struct hlist_node byspi;
    refcount_t refcnt;
    spinlock_t lock;
    struct xfrm_id id;
    struct xfrm_selector sel;
    struct xfrm_mark mark;
    u32 if_id;
    u32 tfcpad;
    u32 genid;
    struct xfrm_state_walk km;
    struct (anon) props;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_algo_auth *aalg;
    struct xfrm_algo *ealg;
    struct xfrm_algo *calg;
    struct xfrm_algo_aead *aead;
    const char *geniv;
    struct xfrm_encap_tmpl *encap;
    xfrm_address_t *coaddr;
    struct xfrm_state *tunnel;
    atomic_t tunnel_users;
    struct xfrm_replay_state replay;
    struct xfrm_replay_state_esn *replay_esn;
    struct xfrm_replay_state preplay;
    struct xfrm_replay_state_esn *preplay_esn;
    const struct xfrm_replay *repl;
    u32 xflags;
    u32 replay_maxage;
    u32 replay_maxdiff;
    struct timer_list rtimer;
    struct xfrm_stats stats;
    struct xfrm_lifetime_cur curlft;
    struct hrtimer mtimer;
    struct xfrm_state_offload xso;
    long int saved_tmo;
    time64_t lastused;
    struct page_frag xfrag;
    const struct xfrm_type *type;
    struct xfrm_mode inner_mode;
    struct xfrm_mode inner_mode_iaf;
    struct xfrm_mode outer_mode;
    const struct xfrm_type_offload *type_offload;
    struct xfrm_sec_ctx *security;
    void *data;
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
<b>Field type changed. </b>
<code>struct xfrm_replay *repl</code> ➡️ <code>const struct xfrm_replay *repl</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct xfrm_state_offload xso</code>
</li>
<li>
<b>Field added. </b>
<code>struct page_frag xfrag</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type_offload *type_offload</code>
</li>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 if_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int lastused</code> ➡️ <code>time64_t lastused</code>
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
<code>struct tasklet_hrtimer mtimer</code> ➡️ <code>struct hrtimer mtimer</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct xfrm_mode *inner_mode</code> ➡️ <code>struct xfrm_mode inner_mode</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct xfrm_mode *inner_mode_iaf</code> ➡️ <code>struct xfrm_mode inner_mode_iaf</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct xfrm_mode *outer_mode</code> ➡️ <code>struct xfrm_mode outer_mode</code>
</li>
</ul>
</details>
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
<code>struct sock *encap_sk</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>struct hlist_node byseq</code>
</li>
<li>
<b>Field added. </b>
<code>__be16 new_mapping_sport</code>
</li>
<li>
<b>Field added. </b>
<code>u32 new_mapping</code>
</li>
<li>
<b>Field added. </b>
<code>u32 mapping_maxage</code>
</li>
<li>
<b>Field added. </b>
<code>enum xfrm_replay_mode repl_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct xfrm_replay *repl</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct xfrm_state_offload xso</code> ➡️ <code>struct xfrm_dev_offload xso</code>
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

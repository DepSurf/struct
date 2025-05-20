# Struct: <code>ifmcaddr6</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    atomic_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    atomic_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    atomic_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct delayed_work mca_work;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct delayed_work mca_work;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct delayed_work mca_work;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct delayed_work mca_work;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct delayed_work mca_work;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct delayed_work mca_work;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
    struct callback_head rcu;
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
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
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
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ifmcaddr6 {
    struct in6_addr mca_addr;
    struct inet6_dev *idev;
    struct ifmcaddr6 *next;
    struct ip6_sf_list *mca_sources;
    struct ip6_sf_list *mca_tomb;
    unsigned int mca_sfmode;
    unsigned char mca_crcount;
    long unsigned int mca_sfcount[2];
    struct timer_list mca_timer;
    unsigned int mca_flags;
    int mca_users;
    refcount_t mca_refcnt;
    spinlock_t mca_lock;
    long unsigned int mca_cstamp;
    long unsigned int mca_tstamp;
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
<code>atomic_t mca_refcnt</code> ➡️ <code>refcount_t mca_refcnt</code>
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
<b>Field added. </b>
<code>struct delayed_work mca_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list mca_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t mca_lock</code>
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

# Struct: <code>key</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct key {
    atomic_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time_t expiry;
    time_t revoked_at;
    time_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    int reject_error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct key {
    atomic_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time_t expiry;
    time_t revoked_at;
    time_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    int reject_error;
    int (*restrict_link)(struct key *, const struct key_type *, const union key_payload *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct key {
    atomic_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time_t expiry;
    time_t revoked_at;
    time_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    int reject_error;
    int (*restrict_link)(struct key *, const struct key_type *, const union key_payload *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time_t expiry;
    time_t revoked_at;
    time_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    int reject_error;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    struct key_type *type;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct watch_list *watchers;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
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
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
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
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct key {
    refcount_t usage;
    key_serial_t serial;
    struct list_head graveyard_link;
    struct rb_node serial_node;
    struct rw_semaphore sem;
    struct key_user *user;
    void *security;
    time64_t expiry;
    time64_t revoked_at;
    time64_t last_used_at;
    kuid_t uid;
    kgid_t gid;
    key_perm_t perm;
    short unsigned int quotalen;
    short unsigned int datalen;
    short int state;
    long unsigned int flags;
    struct keyring_index_key index_key;
    long unsigned int hash;
    long unsigned int len_desc;
    struct key_type *type;
    struct key_tag *domain_tag;
    char *description;
    union key_payload payload;
    struct list_head name_link;
    struct assoc_array keys;
    struct key_restriction *restrict_link;
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
<code>int (*restrict_link)(struct key *, const struct key_type *, const union key_payload *)</code>
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
<b>Field type changed. </b>
<code>atomic_t usage</code> ➡️ <code>refcount_t usage</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*restrict_link)(struct key *, const struct key_type *, const union key_payload *)</code> ➡️ <code>struct key_restriction *restrict_link</code>
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
<code>short int state</code>
</li>
<li>
<b>Field removed. </b>
<code>int reject_error</code>
</li>
<li>
<b>Field type changed. </b>
<code>time_t expiry</code> ➡️ <code>time64_t expiry</code>
</li>
<li>
<b>Field type changed. </b>
<code>time_t revoked_at</code> ➡️ <code>time64_t revoked_at</code>
</li>
<li>
<b>Field type changed. </b>
<code>time_t last_used_at</code> ➡️ <code>time64_t last_used_at</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int hash</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int len_desc</code>
</li>
<li>
<b>Field added. </b>
<code>struct key_tag *domain_tag</code>
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
<code>struct watch_list *watchers</code>
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

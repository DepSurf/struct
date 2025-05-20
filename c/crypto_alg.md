# Struct: <code>crypto_alg</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    atomic_t cra_refcnt;
    char cra_name[64];
    char cra_driver_name[64];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    atomic_t cra_refcnt;
    char cra_name[64];
    char cra_driver_name[64];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    atomic_t cra_refcnt;
    char cra_name[64];
    char cra_driver_name[64];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    atomic_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    atomic_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
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
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
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
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct crypto_alg {
    struct list_head cra_list;
    struct list_head cra_users;
    u32 cra_flags;
    unsigned int cra_blocksize;
    unsigned int cra_ctxsize;
    unsigned int cra_alignmask;
    int cra_priority;
    refcount_t cra_refcnt;
    char cra_name[128];
    char cra_driver_name[128];
    const struct crypto_type *cra_type;
    union (anon) cra_u;
    int (*cra_init)(struct crypto_tfm *);
    void (*cra_exit)(struct crypto_tfm *);
    void (*cra_destroy)(struct crypto_alg *);
    struct module *cra_module;
    union (anon) stats;
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
<code>char cra_name[64]</code> ➡️ <code>char cra_name[128]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char cra_driver_name[64]</code> ➡️ <code>char cra_driver_name[128]</code>
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
<b>Field type changed. </b>
<code>atomic_t cra_refcnt</code> ➡️ <code>refcount_t cra_refcnt</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>union (anon) stats</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>union (anon) stats</code>
</li>
</ul>
</details>
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

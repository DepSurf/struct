# Struct: <code>zswap_pool</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct callback_head callback_head;
    struct notifier_block notifier;
    char tfm_name[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct notifier_block notifier;
    char tfm_name[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
    struct list_head lru;
    spinlock_t lru_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool * zpools[32];
    struct crypto_acomp_ctx *acomp_ctx;
    struct kref kref;
    struct list_head list;
    struct work_struct release_work;
    struct work_struct shrink_work;
    struct hlist_node node;
    char tfm_name[128];
    struct list_lru list_lru;
    struct mem_cgroup *next_shrink;
    struct shrinker *shrinker;
    atomic_t nr_stored;
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
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
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
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct zswap_pool {
    struct zpool *zpool;
    struct crypto_comp **tfm;
    struct kref kref;
    struct list_head list;
    struct work_struct work;
    struct hlist_node node;
    char tfm_name[128];
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
<code>struct work_struct work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head callback_head</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct notifier_block notifier</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char tfm_name[64]</code> ➡️ <code>char tfm_name[128]</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct work_struct release_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct shrink_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct work</code>
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
<code>struct crypto_acomp_ctx *acomp_ctx</code>
</li>
<li>
<b>Field removed. </b>
<code>struct crypto_comp **tfm</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>struct list_head lru</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lru_lock</code>
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
<code>struct zpool * zpools[32]</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_lru list_lru</code>
</li>
<li>
<b>Field added. </b>
<code>struct mem_cgroup *next_shrink</code>
</li>
<li>
<b>Field added. </b>
<code>struct shrinker *shrinker</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t nr_stored</code>
</li>
<li>
<b>Field removed. </b>
<code>struct zpool *zpool</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head lru</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lru_lock</code>
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

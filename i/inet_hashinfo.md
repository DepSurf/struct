# Struct: <code>inet_hashinfo</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    struct kmem_cache *bind2_bucket_cachep;
    struct inet_bind_hashbucket *bhash2;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    bool pernet;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    struct kmem_cache *bind2_bucket_cachep;
    struct inet_bind_hashbucket *bhash2;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    bool pernet;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    struct kmem_cache *bind2_bucket_cachep;
    struct inet_bind_hashbucket *bhash2;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    bool pernet;
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
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
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
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_hashinfo {
    struct inet_ehash_bucket *ehash;
    spinlock_t *ehash_locks;
    unsigned int ehash_mask;
    unsigned int ehash_locks_mask;
    struct kmem_cache *bind_bucket_cachep;
    struct inet_bind_hashbucket *bhash;
    unsigned int bhash_size;
    unsigned int lhash2_mask;
    struct inet_listen_hashbucket *lhash2;
    struct inet_listen_hashbucket listening_hash[32];
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
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
<code>unsigned int lhash2_mask</code>
</li>
<li>
<b>Field added. </b>
<code>struct inet_listen_hashbucket *lhash2</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct inet_listen_hashbucket listening_hash[32]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kmem_cache *bind2_bucket_cachep</code>
</li>
<li>
<b>Field added. </b>
<code>struct inet_bind_hashbucket *bhash2</code>
</li>
<li>
<b>Field added. </b>
<code>bool pernet</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

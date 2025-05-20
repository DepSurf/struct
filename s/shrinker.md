# Struct: <code>shrinker</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    int seeks;
    long int batch;
    long unsigned int flags;
    struct list_head list;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    int seeks;
    long int batch;
    long unsigned int flags;
    struct list_head list;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    int seeks;
    long int batch;
    long unsigned int flags;
    struct list_head list;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    int seeks;
    long int batch;
    long unsigned int flags;
    struct list_head list;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    int seeks;
    long int batch;
    long unsigned int flags;
    struct list_head list;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    int seeks;
    long int batch;
    long unsigned int flags;
    struct list_head list;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    refcount_t refcount;
    struct completion done;
    struct callback_head rcu;
    void *private_data;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
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
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
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
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct shrinker {
    long unsigned int (*count_objects)(struct shrinker *, struct shrink_control *);
    long unsigned int (*scan_objects)(struct shrinker *, struct shrink_control *);
    long int batch;
    int seeks;
    unsigned int flags;
    struct list_head list;
    int id;
    atomic_long_t *nr_deferred;
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int id</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int flags</code> ➡️ <code>unsigned int flags</code>
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>refcount_t refcount</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion done</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field added. </b>
<code>void *private_data</code>
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

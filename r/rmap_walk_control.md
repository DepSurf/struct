# Struct: <code>rmap_walk_control</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    int (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    int (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    int (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool try_lock;
    bool contended;
    bool (*rmap_one)(struct folio *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct folio *);
    struct anon_vma * (*anon_lock)(struct folio *, struct rmap_walk_control *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool try_lock;
    bool contended;
    bool (*rmap_one)(struct folio *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct folio *);
    struct anon_vma * (*anon_lock)(struct folio *, struct rmap_walk_control *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool try_lock;
    bool contended;
    bool (*rmap_one)(struct folio *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct folio *);
    struct anon_vma * (*anon_lock)(struct folio *, struct rmap_walk_control *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool try_lock;
    bool contended;
    bool (*rmap_one)(struct folio *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct folio *);
    struct anon_vma * (*anon_lock)(struct folio *, struct rmap_walk_control *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
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
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
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
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rmap_walk_control {
    void *arg;
    bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *);
    int (*done)(struct page *);
    struct anon_vma * (*anon_lock)(struct page *);
    bool (*invalid_vma)(struct vm_area_struct *, void *);
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
<code>int (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *)</code> ➡️ <code>bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *)</code>
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
<b>Field added. </b>
<code>bool try_lock</code>
</li>
<li>
<b>Field added. </b>
<code>bool contended</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*rmap_one)(struct page *, struct vm_area_struct *, long unsigned int, void *)</code> ➡️ <code>bool (*rmap_one)(struct folio *, struct vm_area_struct *, long unsigned int, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*done)(struct page *)</code> ➡️ <code>int (*done)(struct folio *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct anon_vma * (*anon_lock)(struct page *)</code> ➡️ <code>struct anon_vma * (*anon_lock)(struct folio *, struct rmap_walk_control *)</code>
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

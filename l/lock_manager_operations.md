# Struct: <code>lock_manager_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct lock_manager_operations {
    int (*lm_compare_owner)(struct file_lock *, struct file_lock *);
    long unsigned int (*lm_owner_key)(struct file_lock *);
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct lock_manager_operations {
    void *lm_mod_owner;
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
    bool (*lm_lock_expirable)(struct file_lock *);
    void (*lm_expire_lock)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct lock_manager_operations {
    void *lm_mod_owner;
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
    bool (*lm_lock_expirable)(struct file_lock *);
    void (*lm_expire_lock)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct lock_manager_operations {
    void *lm_mod_owner;
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
    bool (*lm_lock_expirable)(struct file_lock *);
    void (*lm_expire_lock)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct lock_manager_operations {
    void *lm_mod_owner;
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
    bool (*lm_breaker_owns_lease)(struct file_lock *);
    bool (*lm_lock_expirable)(struct file_lock *);
    void (*lm_expire_lock)();
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
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
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
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct lock_manager_operations {
    fl_owner_t (*lm_get_owner)(fl_owner_t);
    void (*lm_put_owner)(fl_owner_t);
    void (*lm_notify)(struct file_lock *);
    int (*lm_grant)(struct file_lock *, int);
    bool (*lm_break)(struct file_lock *);
    int (*lm_change)(struct file_lock *, int, struct list_head *);
    void (*lm_setup)(struct file_lock *, void **);
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*lm_compare_owner)(struct file_lock *, struct file_lock *)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int (*lm_owner_key)(struct file_lock *)</code>
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
<code>bool (*lm_breaker_owns_lease)(struct file_lock *)</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *lm_mod_owner</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*lm_lock_expirable)(struct file_lock *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*lm_expire_lock)()</code>
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

# Struct: <code>mmu_notifier_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    void (*invalidate_page)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    void (*invalidate_page)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    void (*invalidate_page)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    int flags;
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*arch_invalidate_secondary_tlbs)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
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
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
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
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmu_notifier_ops {
    void (*release)(struct mmu_notifier *, struct mm_struct *);
    int (*clear_flush_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*clear_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*test_young)(struct mmu_notifier *, struct mm_struct *, long unsigned int);
    void (*change_pte)(struct mmu_notifier *, struct mm_struct *, long unsigned int, pte_t);
    int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *);
    void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int);
    struct mmu_notifier * (*alloc_notifier)(struct mm_struct *);
    void (*free_notifier)(struct mmu_notifier *);
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
<b>Field removed. </b>
<code>void (*invalidate_page)(struct mmu_notifier *, struct mm_struct *, long unsigned int)</code>
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
<code>int flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*invalidate_range_start)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int)</code> ➡️ <code>int (*invalidate_range_start)(struct mmu_notifier *, const struct mmu_notifier_range *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*invalidate_range_end)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int)</code> ➡️ <code>void (*invalidate_range_end)(struct mmu_notifier *, const struct mmu_notifier_range *)</code>
</li>
</ul>
</details>
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
<code>struct mmu_notifier * (*alloc_notifier)(struct mm_struct *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_notifier)(struct mmu_notifier *)</code>
</li>
</ul>
</details>
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
<code>void (*arch_invalidate_secondary_tlbs)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*invalidate_range)(struct mmu_notifier *, struct mm_struct *, long unsigned int, long unsigned int)</code>
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

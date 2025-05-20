# Struct: <code>hmm_mirror_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*sync_cpu_device_pagetables)(struct hmm_mirror *, enum hmm_update_type, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    void (*sync_cpu_device_pagetables)(struct hmm_mirror *, enum hmm_update_type, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct hmm_update *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct hmm_update *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
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
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hmm_mirror_ops {
    void (*release)(struct hmm_mirror *);
    int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *);
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*release)(struct hmm_mirror *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*sync_cpu_device_pagetables)(struct hmm_mirror *, enum hmm_update_type, long unsigned int, long unsigned int)</code> ➡️ <code>int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct hmm_update *)</code>
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
<b>Field type changed. </b>
<code>int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct hmm_update *)</code> ➡️ <code>int (*sync_cpu_device_pagetables)(struct hmm_mirror *, const struct mmu_notifier_range *)</code>
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

# Struct: <code>kvm_arch_memory_slot</code>

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
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int * gfn_track[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int * gfn_track[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int * gfn_track[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int * gfn_track[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int * gfn_track[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int * gfn_track[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    struct kvm_rmap_head * rmap[3];
    struct kvm_lpage_info * lpage_info[2];
    short unsigned int *gfn_write_track;
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
struct kvm_arch_memory_slot {
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kvm_arch_memory_slot {
    long unsigned int *rmap;
};
```
</details>
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>short unsigned int *gfn_write_track</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int * gfn_track[1]</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>

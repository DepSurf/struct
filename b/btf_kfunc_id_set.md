# Struct: <code>btf_kfunc_id_set</code>

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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct btf_kfunc_id_set {
    struct module *owner;
    struct btf_id_set *check_set;
    struct btf_id_set *acquire_set;
    struct btf_id_set *release_set;
    struct btf_id_set *ret_null_set;
    struct btf_id_set *kptr_acquire_set;
    struct btf_id_set * sets[5];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct btf_kfunc_id_set {
    struct module *owner;
    struct btf_id_set8 *set;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct btf_kfunc_id_set {
    struct module *owner;
    struct btf_id_set8 *set;
    btf_kfunc_filter_t filter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct btf_kfunc_id_set {
    struct module *owner;
    struct btf_id_set8 *set;
    btf_kfunc_filter_t filter;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct btf_id_set8 *set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct btf_id_set *check_set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct btf_id_set *acquire_set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct btf_id_set *release_set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct btf_id_set *ret_null_set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct btf_id_set *kptr_acquire_set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct btf_id_set * sets[5]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>btf_kfunc_filter_t filter</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

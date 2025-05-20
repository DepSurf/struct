# Struct: <code>nh_group</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool mpath;
    bool fdb_nh;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool mpath;
    bool fdb_nh;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool is_multipath;
    bool hash_threshold;
    bool resilient;
    bool fdb_nh;
    bool has_v4;
    struct nh_res_table *res_table;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool is_multipath;
    bool hash_threshold;
    bool resilient;
    bool fdb_nh;
    bool has_v4;
    struct nh_res_table *res_table;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool is_multipath;
    bool hash_threshold;
    bool resilient;
    bool fdb_nh;
    bool has_v4;
    struct nh_res_table *res_table;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool is_multipath;
    bool hash_threshold;
    bool resilient;
    bool fdb_nh;
    bool has_v4;
    struct nh_res_table *res_table;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool is_multipath;
    bool hash_threshold;
    bool resilient;
    bool fdb_nh;
    bool has_v4;
    struct nh_res_table *res_table;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nh_group {
    struct nh_group *spare;
    u16 num_nh;
    bool is_multipath;
    bool hash_threshold;
    bool resilient;
    bool fdb_nh;
    bool has_v4;
    struct nh_res_table *res_table;
    struct nh_grp_entry nh_entries[0];
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
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
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
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nh_group {
    u16 num_nh;
    bool mpath;
    bool has_v4;
    struct nh_grp_entry nh_entries[0];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct nh_group *spare</code>
</li>
<li>
<b>Field added. </b>
<code>bool fdb_nh</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool is_multipath</code>
</li>
<li>
<b>Field added. </b>
<code>bool hash_threshold</code>
</li>
<li>
<b>Field added. </b>
<code>bool resilient</code>
</li>
<li>
<b>Field added. </b>
<code>struct nh_res_table *res_table</code>
</li>
<li>
<b>Field removed. </b>
<code>bool mpath</code>
</li>
</ul>
</details>
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

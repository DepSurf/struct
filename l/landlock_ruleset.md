# Struct: <code>landlock_ruleset</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct landlock_ruleset {
    struct rb_root root;
    struct landlock_hierarchy *hierarchy;
    struct work_struct work_free;
    struct mutex lock;
    refcount_t usage;
    u32 num_rules;
    u32 num_layers;
    u16 fs_access_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct landlock_ruleset {
    struct rb_root root;
    struct landlock_hierarchy *hierarchy;
    struct work_struct work_free;
    struct mutex lock;
    refcount_t usage;
    u32 num_rules;
    u32 num_layers;
    u16 fs_access_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct landlock_ruleset {
    struct rb_root root;
    struct landlock_hierarchy *hierarchy;
    struct work_struct work_free;
    struct mutex lock;
    refcount_t usage;
    u32 num_rules;
    u32 num_layers;
    access_mask_t fs_access_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct landlock_ruleset {
    struct rb_root root;
    struct landlock_hierarchy *hierarchy;
    struct work_struct work_free;
    struct mutex lock;
    refcount_t usage;
    u32 num_rules;
    u32 num_layers;
    access_mask_t fs_access_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct landlock_ruleset {
    struct rb_root root;
    struct landlock_hierarchy *hierarchy;
    struct work_struct work_free;
    struct mutex lock;
    refcount_t usage;
    u32 num_rules;
    u32 num_layers;
    access_mask_t fs_access_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct landlock_ruleset {
    struct rb_root root_inode;
    struct rb_root root_net_port;
    struct landlock_hierarchy *hierarchy;
    struct work_struct work_free;
    struct mutex lock;
    refcount_t usage;
    u32 num_rules;
    u32 num_layers;
    access_masks_t access_masks[0];
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u16 fs_access_masks[0]</code> ➡️ <code>access_mask_t fs_access_masks[0]</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rb_root root_inode</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_root root_net_port</code>
</li>
<li>
<b>Field added. </b>
<code>access_masks_t access_masks[0]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_root root</code>
</li>
<li>
<b>Field removed. </b>
<code>access_mask_t fs_access_masks[0]</code>
</li>
</ul>
</details>
</li>
</ul>

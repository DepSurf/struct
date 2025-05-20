# Struct: <code>rdtgroup</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    int closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rdtgroup {
    struct kernfs_node *kn;
    struct list_head rdtgroup_list;
    u32 closid;
    struct cpumask cpu_mask;
    int flags;
    atomic_t waitcount;
    enum rdt_group_type type;
    struct mongroup mon;
    enum rdtgrp_mode mode;
    struct pseudo_lock_region *plr;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum rdt_group_type type</code>
</li>
<li>
<b>Field added. </b>
<code>struct mongroup mon</code>
</li>
<li>
<b>Field type changed. </b>
<code>int closid</code> ➡️ <code>u32 closid</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum rdtgrp_mode mode</code>
</li>
<li>
<b>Field added. </b>
<code>struct pseudo_lock_region *plr</code>
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
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

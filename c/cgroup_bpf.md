# Struct: <code>cgroup_bpf</code>

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
struct cgroup_bpf {
    struct bpf_prog * prog[3];
    struct bpf_prog * effective[3];
    bool disallow_override[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog * prog[4];
    struct bpf_prog * effective[4];
    bool disallow_override[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[7];
    struct list_head progs[7];
    u32 flags[7];
    struct bpf_prog_array *inactive;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[17];
    struct list_head progs[17];
    u32 flags[17];
    struct bpf_prog_array *inactive;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[18];
    struct list_head progs[18];
    u32 flags[18];
    struct bpf_prog_array *inactive;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[34];
    struct list_head progs[34];
    u32 flags[34];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[38];
    struct list_head progs[38];
    u32 flags[38];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[39];
    struct list_head progs[39];
    u32 flags[39];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[33];
    struct hlist_head progs[33];
    u8 flags[33];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[33];
    struct hlist_head progs[33];
    u8 flags[33];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[38];
    struct hlist_head progs[38];
    u8 flags[38];
    struct list_head storages;
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
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
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
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
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cgroup_bpf {
    struct bpf_prog_array * effective[23];
    struct list_head progs[23];
    u32 flags[23];
    struct bpf_prog_array *inactive;
    struct percpu_ref refcnt;
    struct work_struct release_work;
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
<b>Field type changed. </b>
<code>struct bpf_prog * prog[3]</code> ➡️ <code>struct bpf_prog * prog[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog * effective[3]</code> ➡️ <code>struct bpf_prog * effective[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool disallow_override[3]</code> ➡️ <code>bool disallow_override[4]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head progs[7]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 flags[7]</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_prog_array *inactive</code>
</li>
<li>
<b>Field removed. </b>
<code>struct bpf_prog * prog[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>bool disallow_override[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog * effective[4]</code> ➡️ <code>struct bpf_prog_array * effective[7]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[7]</code> ➡️ <code>struct bpf_prog_array * effective[17]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[7]</code> ➡️ <code>struct list_head progs[17]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[7]</code> ➡️ <code>u32 flags[17]</code>
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
<code>struct bpf_prog_array * effective[17]</code> ➡️ <code>struct bpf_prog_array * effective[18]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[17]</code> ➡️ <code>struct list_head progs[18]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[17]</code> ➡️ <code>u32 flags[18]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct percpu_ref refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct release_work</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[18]</code> ➡️ <code>struct bpf_prog_array * effective[23]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[18]</code> ➡️ <code>struct list_head progs[23]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[18]</code> ➡️ <code>u32 flags[23]</code>
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
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[23]</code> ➡️ <code>struct bpf_prog_array * effective[34]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[23]</code> ➡️ <code>struct list_head progs[34]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[23]</code> ➡️ <code>u32 flags[34]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head storages</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[34]</code> ➡️ <code>struct bpf_prog_array * effective[38]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[34]</code> ➡️ <code>struct list_head progs[38]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[34]</code> ➡️ <code>u32 flags[38]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[38]</code> ➡️ <code>struct bpf_prog_array * effective[39]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[38]</code> ➡️ <code>struct list_head progs[39]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[38]</code> ➡️ <code>u32 flags[39]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[39]</code> ➡️ <code>struct bpf_prog_array * effective[23]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[39]</code> ➡️ <code>struct list_head progs[23]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[39]</code> ➡️ <code>u32 flags[23]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[23]</code> ➡️ <code>struct bpf_prog_array * effective[33]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head progs[23]</code> ➡️ <code>struct hlist_head progs[33]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags[23]</code> ➡️ <code>u8 flags[33]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bpf_prog_array * effective[33]</code> ➡️ <code>struct bpf_prog_array * effective[38]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hlist_head progs[33]</code> ➡️ <code>struct hlist_head progs[38]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 flags[33]</code> ➡️ <code>u8 flags[38]</code>
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

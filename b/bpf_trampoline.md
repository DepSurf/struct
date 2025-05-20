# Struct: <code>bpf_trampoline</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct mutex mutex;
    refcount_t refcnt;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    void *image;
    u64 selector;
    struct bpf_ksym ksym;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct mutex mutex;
    refcount_t refcnt;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    u64 selector;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct mutex mutex;
    refcount_t refcnt;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    u64 selector;
    struct module *mod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct mutex mutex;
    refcount_t refcnt;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    u64 selector;
    struct module *mod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct mutex mutex;
    refcount_t refcnt;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    u64 selector;
    struct module *mod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct ftrace_ops *fops;
    struct mutex mutex;
    refcount_t refcnt;
    u32 flags;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    u64 selector;
    struct module *mod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct ftrace_ops *fops;
    struct mutex mutex;
    refcount_t refcnt;
    u32 flags;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    struct module *mod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_trampoline {
    struct hlist_node hlist;
    struct ftrace_ops *fops;
    struct mutex mutex;
    refcount_t refcnt;
    u32 flags;
    u64 key;
    struct (anon) func;
    struct bpf_prog *extension_prog;
    struct hlist_head progs_hlist[3];
    int progs_cnt[3];
    struct bpf_tramp_image *cur_image;
    struct module *mod;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_tramp_image *cur_image</code>
</li>
<li>
<b>Field removed. </b>
<code>void *image</code>
</li>
<li>
<b>Field removed. </b>
<code>struct bpf_ksym ksym</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct module *mod</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ftrace_ops *fops</code>
</li>
<li>
<b>Field added. </b>
<code>u32 flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 selector</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

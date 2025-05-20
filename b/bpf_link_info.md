# Struct: <code>bpf_link_info</code>

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
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) netns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
    struct (anon) struct_ops;
    struct (anon) netfilter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_link_info {
    __u32 type;
    __u32 id;
    __u32 prog_id;
    struct (anon) raw_tracepoint;
    struct (anon) tracing;
    struct (anon) cgroup;
    struct (anon) iter;
    struct (anon) netns;
    struct (anon) xdp;
    struct (anon) struct_ops;
    struct (anon) netfilter;
    struct (anon) kprobe_multi;
    struct (anon) uprobe_multi;
    struct (anon) perf_event;
    struct (anon) tcx;
    struct (anon) netkit;
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
<code>struct (anon) iter</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) xdp</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) struct_ops</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) netfilter</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) kprobe_multi</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) uprobe_multi</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) perf_event</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) tcx</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) netkit</code>
</li>
</ul>
</details>
</li>
</ul>

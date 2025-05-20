# Struct: <code>bpf_tracing_link</code>

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
struct bpf_tracing_link {
    struct bpf_link link;
    enum bpf_attach_type attach_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_tramp_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_tramp_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_tramp_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_tracing_link {
    struct bpf_tramp_link link;
    enum bpf_attach_type attach_type;
    struct bpf_trampoline *trampoline;
    struct bpf_prog *tgt_prog;
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
<code>struct bpf_trampoline *trampoline</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_prog *tgt_prog</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bpf_link link</code> ➡️ <code>struct bpf_tramp_link link</code>
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

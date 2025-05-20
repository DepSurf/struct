# Struct: <code>bpf_subprog_info</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
    bool is_async_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
    bool is_async_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
    bool is_async_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
    bool is_async_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
    bool has_tail_call;
    bool tail_call_reachable;
    bool has_ld_abs;
    bool is_cb;
    bool is_async_cb;
    bool is_exception_cb;
    bool args_cached;
    u8 arg_cnt;
    struct bpf_subprog_arg_info args[5];
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
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
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
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_subprog_info {
    u32 start;
    u32 linfo_idx;
    u16 stack_depth;
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
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 linfo_idx</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool has_tail_call</code>
</li>
<li>
<b>Field added. </b>
<code>bool tail_call_reachable</code>
</li>
<li>
<b>Field added. </b>
<code>bool has_ld_abs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool is_async_cb</code>
</li>
</ul>
</details>
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
<code>bool is_cb</code>
</li>
<li>
<b>Field added. </b>
<code>bool is_exception_cb</code>
</li>
<li>
<b>Field added. </b>
<code>bool args_cached</code>
</li>
<li>
<b>Field added. </b>
<code>u8 arg_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_subprog_arg_info args[5]</code>
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

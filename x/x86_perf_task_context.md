# Struct: <code>x86_perf_task_context</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int lbr_callstack_users;
    int lbr_stack_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int lbr_callstack_users;
    int lbr_stack_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int lbr_callstack_users;
    int lbr_stack_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int lbr_callstack_users;
    int lbr_stack_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int lbr_callstack_users;
    int lbr_stack_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_sel;
    int tos;
    int valid_lbrs;
    struct x86_perf_task_context_opt opt;
    struct lbr_entry lbr[32];
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
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct x86_perf_task_context {
    u64 lbr_from[32];
    u64 lbr_to[32];
    u64 lbr_info[32];
    int tos;
    int valid_lbrs;
    int lbr_callstack_users;
    int lbr_stack_state;
    int log_id;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int valid_lbrs</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int log_id</code>
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
<code>u64 lbr_sel</code>
</li>
<li>
<b>Field added. </b>
<code>struct x86_perf_task_context_opt opt</code>
</li>
<li>
<b>Field added. </b>
<code>struct lbr_entry lbr[32]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 lbr_from[32]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 lbr_to[32]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 lbr_info[32]</code>
</li>
<li>
<b>Field removed. </b>
<code>int lbr_callstack_users</code>
</li>
<li>
<b>Field removed. </b>
<code>int lbr_stack_state</code>
</li>
<li>
<b>Field removed. </b>
<code>int log_id</code>
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

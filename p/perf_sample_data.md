# Struct: <code>perf_sample_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    u64 aux_size;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
    u64 cgroup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    u64 aux_size;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
    u64 cgroup;
    u64 data_page_size;
    u64 code_page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    union perf_sample_weight weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    u64 aux_size;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
    u64 cgroup;
    u64 data_page_size;
    u64 code_page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    union perf_sample_weight weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    u64 aux_size;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
    u64 cgroup;
    u64 data_page_size;
    u64 code_page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    union perf_sample_weight weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    u64 aux_size;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
    u64 cgroup;
    u64 data_page_size;
    u64 code_page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 sample_flags;
    u64 period;
    struct perf_branch_stack *br_stack;
    union perf_sample_weight weight;
    union perf_mem_data_src data_src;
    u64 txn;
    u64 addr;
    struct perf_raw_record *raw;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    u64 aux_size;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
    u64 cgroup;
    u64 data_page_size;
    u64 code_page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 sample_flags;
    u64 period;
    u64 dyn_size;
    u64 type;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    struct (anon) cpu_entry;
    u64 ip;
    struct perf_callchain_entry *callchain;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    union perf_sample_weight weight;
    union perf_mem_data_src data_src;
    u64 txn;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 stream_id;
    u64 cgroup;
    u64 addr;
    u64 phys_addr;
    u64 data_page_size;
    u64 code_page_size;
    u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 sample_flags;
    u64 period;
    u64 dyn_size;
    u64 type;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    struct (anon) cpu_entry;
    u64 ip;
    struct perf_callchain_entry *callchain;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 *br_stack_cntr;
    union perf_sample_weight weight;
    union perf_mem_data_src data_src;
    u64 txn;
    struct perf_regs regs_user;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 stream_id;
    u64 cgroup;
    u64 addr;
    u64 phys_addr;
    u64 data_page_size;
    u64 code_page_size;
    u64 aux_size;
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
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
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
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct perf_sample_data {
    u64 addr;
    struct perf_raw_record *raw;
    struct perf_branch_stack *br_stack;
    u64 period;
    u64 weight;
    u64 txn;
    union perf_mem_data_src data_src;
    u64 type;
    u64 ip;
    struct (anon) tid_entry;
    u64 time;
    u64 id;
    u64 stream_id;
    struct (anon) cpu_entry;
    struct perf_callchain_entry *callchain;
    struct perf_regs regs_user;
    struct pt_regs regs_user_copy;
    struct perf_regs regs_intr;
    u64 stack_user_size;
    u64 phys_addr;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 phys_addr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 aux_size</code>
</li>
<li>
<b>Field added. </b>
<code>u64 cgroup</code>
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
<code>u64 data_page_size</code>
</li>
<li>
<b>Field added. </b>
<code>u64 code_page_size</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pt_regs regs_user_copy</code>
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
<code>u64 weight</code> ➡️ <code>union perf_sample_weight weight</code>
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
<code>u64 sample_flags</code>
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
<code>u64 dyn_size</code>
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
<code>u64 *br_stack_cntr</code>
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

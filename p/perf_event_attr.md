# Struct: <code>perf_event_attr</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 config1;
    __u64 bp_len;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u32 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 config1;
    __u64 bp_len;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 config1;
    __u64 bp_len;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 config1;
    __u64 bp_len;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 config1;
    __u64 bp_len;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 build_id;
    __u64 inherit_thread;
    __u64 remove_on_exec;
    __u64 sigtrap;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
    __u64 sig_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 build_id;
    __u64 inherit_thread;
    __u64 remove_on_exec;
    __u64 sigtrap;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
    __u64 sig_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 build_id;
    __u64 inherit_thread;
    __u64 remove_on_exec;
    __u64 sigtrap;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
    __u64 sig_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 build_id;
    __u64 inherit_thread;
    __u64 remove_on_exec;
    __u64 sigtrap;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
    __u64 sig_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 build_id;
    __u64 inherit_thread;
    __u64 remove_on_exec;
    __u64 sigtrap;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
    __u64 sig_data;
    __u64 config3;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 cgroup;
    __u64 text_poke;
    __u64 build_id;
    __u64 inherit_thread;
    __u64 remove_on_exec;
    __u64 sigtrap;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
    __u32 aux_sample_size;
    __u32 __reserved_3;
    __u64 sig_data;
    __u64 config3;
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
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
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
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct perf_event_attr {
    __u32 type;
    __u32 size;
    __u64 config;
    __u64 sample_period;
    __u64 sample_freq;
    __u64 sample_type;
    __u64 read_format;
    __u64 disabled;
    __u64 inherit;
    __u64 pinned;
    __u64 exclusive;
    __u64 exclude_user;
    __u64 exclude_kernel;
    __u64 exclude_hv;
    __u64 exclude_idle;
    __u64 mmap;
    __u64 comm;
    __u64 freq;
    __u64 inherit_stat;
    __u64 enable_on_exec;
    __u64 task;
    __u64 watermark;
    __u64 precise_ip;
    __u64 mmap_data;
    __u64 sample_id_all;
    __u64 exclude_host;
    __u64 exclude_guest;
    __u64 exclude_callchain_kernel;
    __u64 exclude_callchain_user;
    __u64 mmap2;
    __u64 comm_exec;
    __u64 use_clockid;
    __u64 context_switch;
    __u64 write_backward;
    __u64 namespaces;
    __u64 ksymbol;
    __u64 bpf_event;
    __u64 aux_output;
    __u64 __reserved_1;
    __u32 wakeup_events;
    __u32 wakeup_watermark;
    __u32 bp_type;
    __u64 bp_addr;
    __u64 kprobe_func;
    __u64 uprobe_path;
    __u64 config1;
    __u64 bp_len;
    __u64 kprobe_addr;
    __u64 probe_offset;
    __u64 config2;
    __u64 branch_sample_type;
    __u64 sample_regs_user;
    __u32 sample_stack_user;
    __s32 clockid;
    __u64 sample_regs_intr;
    __u32 aux_watermark;
    __u16 sample_max_stack;
    __u16 __reserved_2;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 write_backward</code>
</li>
<li>
<b>Field added. </b>
<code>__u16 sample_max_stack</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 __reserved_2</code> ➡️ <code>__u16 __reserved_2</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 namespaces</code>
</li>
</ul>
</details>
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
<code>__u64 kprobe_func</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 uprobe_path</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 kprobe_addr</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 probe_offset</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 ksymbol</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 bpf_event</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 aux_output</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 cgroup</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 aux_sample_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 __reserved_3</code>
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
<code>__u64 text_poke</code>
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
<code>__u64 build_id</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 inherit_thread</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 remove_on_exec</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 sigtrap</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 sig_data</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 config3</code>
</li>
</ul>
</details>
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

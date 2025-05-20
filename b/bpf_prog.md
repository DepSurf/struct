# Struct: <code>bpf_prog</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u32 len;
    enum bpf_prog_type type;
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const struct sk_buff *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u32 len;
    enum bpf_prog_type type;
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const struct sk_buff *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 xdp_adjust_head;
    enum bpf_prog_type type;
    u32 len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 locked;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    enum bpf_prog_type type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 locked;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    enum bpf_prog_type type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 undo_set_mem;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 undo_set_mem;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_stats *stats;
    int *active;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    u16 call_get_func_ip;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_stats *stats;
    int *active;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinding_requested;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    u16 call_get_func_ip;
    u16 tstamp_type_access;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_stats *stats;
    int *active;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    struct (anon) __empty_insns;
    struct sock_filter insns[0];
    struct (anon) __empty_insnsi;
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinding_requested;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    u16 call_get_func_ip;
    u16 tstamp_type_access;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_stats *stats;
    int *active;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    struct (anon) __empty_insns;
    struct sock_filter insns[0];
    struct (anon) __empty_insnsi;
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinding_requested;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    u16 call_get_func_ip;
    u16 tstamp_type_access;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_stats *stats;
    int *active;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    struct (anon) __empty_insns;
    struct sock_filter insns[0];
    struct (anon) __empty_insnsi;
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinding_requested;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    u16 call_get_stack;
    u16 call_get_func_ip;
    u16 tstamp_type_access;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_stats *stats;
    int *active;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    struct (anon) __empty_insns;
    struct sock_filter insns[0];
    struct (anon) __empty_insnsi;
    struct bpf_insn insnsi[0];
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
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
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
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_prog {
    u16 pages;
    u16 jited;
    u16 jit_requested;
    u16 gpl_compatible;
    u16 cb_access;
    u16 dst_needed;
    u16 blinded;
    u16 is_func;
    u16 kprobe_override;
    u16 has_callchain_buf;
    u16 enforce_expected_attach_type;
    enum bpf_prog_type type;
    enum bpf_attach_type expected_attach_type;
    u32 len;
    u32 jited_len;
    u8 tag[8];
    struct bpf_prog_aux *aux;
    struct sock_fprog_kern *orig_prog;
    unsigned int (*bpf_func)(const void *, const struct bpf_insn *);
    struct sock_filter insns[0];
    struct bpf_insn insnsi[0];
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 xdp_adjust_head</code>
</li>
<li>
<b>Field added. </b>
<code>u8 tag[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int (*bpf_func)(const struct sk_buff *, const struct bpf_insn *)</code> ➡️ <code>unsigned int (*bpf_func)(const void *, const struct bpf_insn *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 locked</code>
</li>
<li>
<b>Field added. </b>
<code>u32 jited_len</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 xdp_adjust_head</code>
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
<code>u16 jit_requested</code>
</li>
<li>
<b>Field added. </b>
<code>u16 undo_set_mem</code>
</li>
<li>
<b>Field added. </b>
<code>u16 blinded</code>
</li>
<li>
<b>Field added. </b>
<code>u16 is_func</code>
</li>
<li>
<b>Field added. </b>
<code>u16 kprobe_override</code>
</li>
<li>
<b>Field added. </b>
<code>u16 has_callchain_buf</code>
</li>
<li>
<b>Field added. </b>
<code>enum bpf_attach_type expected_attach_type</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 locked</code>
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
<code>u16 enforce_expected_attach_type</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 undo_set_mem</code>
</li>
</ul>
</details>
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
<code>u16 call_get_stack</code>
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
<code>struct bpf_prog_stats *stats</code>
</li>
<li>
<b>Field added. </b>
<code>int *active</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 call_get_func_ip</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 blinding_requested</code>
</li>
<li>
<b>Field added. </b>
<code>u16 tstamp_type_access</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) __empty_insns</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) __empty_insnsi</code>
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

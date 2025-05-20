# Struct: <code>bpf_verifier_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id);
    bool (*is_valid_access)(int, int, enum bpf_access_type);
    u32 (*convert_ctx_access)(enum bpf_access_type, int, int, int, struct bpf_insn *, struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id);
    bool (*is_valid_access)(int, int, enum bpf_access_type, enum bpf_reg_type *);
    u32 (*convert_ctx_access)(enum bpf_access_type, int, int, int, struct bpf_insn *, struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id);
    bool (*is_valid_access)(int, int, enum bpf_access_type, enum bpf_reg_type *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    u32 (*convert_ctx_access)(enum bpf_access_type, int, int, int, struct bpf_insn *, struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id);
    bool (*is_valid_access)(int, int, enum bpf_access_type, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*test_run)(struct bpf_prog *, const union bpf_attr *, union bpf_attr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id);
    bool (*is_valid_access)(int, int, enum bpf_access_type, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf_type *, int, int, enum bpf_access_type, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *);
    bool (*check_kfunc_call)(u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *);
    bool (*check_kfunc_call)(u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *, enum bpf_type_flag *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct bpf_reg_state *, int, int, enum bpf_access_type, u32 *, enum bpf_type_flag *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct bpf_reg_state *, int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
    int (*btf_struct_access)(struct bpf_verifier_log *, const struct bpf_reg_state *, int, int);
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
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
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
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_verifier_ops {
    const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *);
    bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *);
    int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *);
    int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *);
    u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *);
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
<b>Field type changed. </b>
<code>bool (*is_valid_access)(int, int, enum bpf_access_type)</code> ➡️ <code>bool (*is_valid_access)(int, int, enum bpf_access_type, enum bpf_reg_type *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*gen_prologue)(struct bpf_insn *, bool, const struct bpf_prog *)</code>
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
<code>int (*test_run)(struct bpf_prog *, const union bpf_attr *, union bpf_attr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*is_valid_access)(int, int, enum bpf_access_type, enum bpf_reg_type *)</code> ➡️ <code>bool (*is_valid_access)(int, int, enum bpf_access_type, struct bpf_insn_access_aux *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 (*convert_ctx_access)(enum bpf_access_type, int, int, int, struct bpf_insn *, struct bpf_prog *)</code> ➡️ <code>u32 (*convert_ctx_access)(enum bpf_access_type, const struct bpf_insn *, struct bpf_insn *, struct bpf_prog *, u32 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*test_run)(struct bpf_prog *, const union bpf_attr *, union bpf_attr *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*gen_ld_abs)(const struct bpf_insn *, struct bpf_insn *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id)</code> ➡️ <code>const struct bpf_func_proto * (*get_func_proto)(enum bpf_func_id, const struct bpf_prog *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*is_valid_access)(int, int, enum bpf_access_type, struct bpf_insn_access_aux *)</code> ➡️ <code>bool (*is_valid_access)(int, int, enum bpf_access_type, const struct bpf_prog *, struct bpf_insn_access_aux *)</code>
</li>
</ul>
</details>
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
<code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf_type *, int, int, enum bpf_access_type, u32 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf_type *, int, int, enum bpf_access_type, u32 *)</code> ➡️ <code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *)</code>
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
<code>bool (*check_kfunc_call)(u32)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool (*check_kfunc_call)(u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *)</code> ➡️ <code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *, enum bpf_type_flag *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct btf *, const struct btf_type *, int, int, enum bpf_access_type, u32 *, enum bpf_type_flag *)</code> ➡️ <code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct bpf_reg_state *, int, int, enum bpf_access_type, u32 *, enum bpf_type_flag *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct bpf_reg_state *, int, int, enum bpf_access_type, u32 *, enum bpf_type_flag *)</code> ➡️ <code>int (*btf_struct_access)(struct bpf_verifier_log *, const struct bpf_reg_state *, int, int)</code>
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

# Struct: <code>bpf_struct_ops</code>

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
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *, const struct bpf_prog *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    int (*update)(void *, void *);
    int (*validate)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_struct_ops {
    const struct bpf_verifier_ops *verifier_ops;
    int (*init)(struct btf *);
    int (*check_member)(const struct btf_type *, const struct btf_member *, const struct bpf_prog *);
    int (*init_member)(const struct btf_type *, const struct btf_member *, void *, const void *);
    int (*reg)(void *);
    void (*unreg)(void *);
    int (*update)(void *, void *);
    int (*validate)(void *);
    const struct btf_type *type;
    const struct btf_type *value_type;
    const char *name;
    struct btf_func_model func_models[64];
    u32 type_id;
    u32 value_id;
    void *cfi_stubs;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>int (*update)(void *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*validate)(void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*check_member)(const struct btf_type *, const struct btf_member *)</code> ➡️ <code>int (*check_member)(const struct btf_type *, const struct btf_member *, const struct bpf_prog *)</code>
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
<code>void *cfi_stubs</code>
</li>
</ul>
</details>
</li>
</ul>

# Struct: <code>bpf_jit_poke_descriptor</code>

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
struct bpf_jit_poke_descriptor {
    void *ip;
    struct (anon) tail_call;
    bool ip_stable;
    u8 adj_off;
    u16 reason;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    void *aux;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    void *aux;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    void *aux;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    void *aux;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    void *aux;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_jit_poke_descriptor {
    void *tailcall_target;
    void *tailcall_bypass;
    void *bypass_addr;
    void *aux;
    struct (anon) tail_call;
    bool tailcall_target_stable;
    u8 adj_off;
    u16 reason;
    u32 insn_idx;
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
<code>void *tailcall_target</code>
</li>
<li>
<b>Field added. </b>
<code>void *tailcall_bypass</code>
</li>
<li>
<b>Field added. </b>
<code>void *bypass_addr</code>
</li>
<li>
<b>Field added. </b>
<code>bool tailcall_target_stable</code>
</li>
<li>
<b>Field added. </b>
<code>u32 insn_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>void *ip</code>
</li>
<li>
<b>Field removed. </b>
<code>bool ip_stable</code>
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
<code>void *aux</code>
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

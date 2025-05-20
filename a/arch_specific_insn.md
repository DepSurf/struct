# Struct: <code>arch_specific_insn</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    int boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    int boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    int boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
    int tp_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    unsigned int boostable;
    unsigned char size;
    unsigned char opcode;
    struct (anon) jcc;
    struct (anon) loop;
    struct (anon) indirect;
    s32 rel32;
    void (*emulate_op)(struct kprobe *, struct pt_regs *);
    int tp_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    unsigned int boostable;
    unsigned char size;
    unsigned char opcode;
    struct (anon) jcc;
    struct (anon) loop;
    struct (anon) indirect;
    s32 rel32;
    void (*emulate_op)(struct kprobe *, struct pt_regs *);
    int tp_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    unsigned int boostable;
    unsigned char size;
    unsigned char opcode;
    struct (anon) jcc;
    struct (anon) loop;
    struct (anon) indirect;
    s32 rel32;
    void (*emulate_op)(struct kprobe *, struct pt_regs *);
    int tp_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    unsigned int boostable;
    unsigned char size;
    unsigned char opcode;
    struct (anon) jcc;
    struct (anon) loop;
    struct (anon) indirect;
    s32 rel32;
    void (*emulate_op)(struct kprobe *, struct pt_regs *);
    int tp_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    unsigned int boostable;
    unsigned char size;
    unsigned char opcode;
    struct (anon) jcc;
    struct (anon) loop;
    struct (anon) indirect;
    s32 rel32;
    void (*emulate_op)(struct kprobe *, struct pt_regs *);
    int tp_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    unsigned int boostable;
    unsigned char size;
    unsigned char opcode;
    struct (anon) jcc;
    struct (anon) loop;
    struct (anon) indirect;
    s32 rel32;
    void (*emulate_op)(struct kprobe *, struct pt_regs *);
    int tp_len;
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
struct arch_specific_insn {
    struct arch_probe_insn api;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    int boostable;
};
```
</details>
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
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct arch_specific_insn {
    kprobe_opcode_t *insn;
    bool boostable;
    bool if_modifier;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int boostable</code> ➡️ <code>bool boostable</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int tp_len</code>
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
<code>unsigned char size</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char opcode</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) jcc</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) loop</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) indirect</code>
</li>
<li>
<b>Field added. </b>
<code>s32 rel32</code>
</li>
<li>
<b>Field added. </b>
<code>void (*emulate_op)(struct kprobe *, struct pt_regs *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool if_modifier</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool boostable</code> ➡️ <code>unsigned int boostable</code>
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
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct arch_probe_insn api</code>
</li>
<li>
<b>Field removed. </b>
<code>kprobe_opcode_t *insn</code>
</li>
<li>
<b>Field removed. </b>
<code>bool boostable</code>
</li>
<li>
<b>Field removed. </b>
<code>bool if_modifier</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool if_modifier</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool boostable</code> ➡️ <code>int boostable</code>
</li>
</ul>
</details>
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

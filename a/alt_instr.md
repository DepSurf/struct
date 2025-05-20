# Struct: <code>alt_instr</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u32 cpuid;
    u32 flags;
    u32 ft_flags;
    u8 instrlen;
    u8 replacementlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u32 cpuid;
    u32 flags;
    u32 ft_flags;
    u8 instrlen;
    u8 replacementlen;
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
struct alt_instr {
    s32 orig_offset;
    s32 alt_offset;
    u16 cpufeature;
    u8 orig_len;
    u8 alt_len;
};
```
</details>
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
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct alt_instr {
    s32 instr_offset;
    s32 repl_offset;
    u16 cpuid;
    u8 instrlen;
    u8 replacementlen;
    u8 padlen;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 padlen</code>
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
<code>u32 flags</code>
</li>
<li>
<b>Field added. </b>
<code>u32 ft_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 cpuid</code> ➡️ <code>u32 cpuid</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s32 orig_offset</code>
</li>
<li>
<b>Field added. </b>
<code>s32 alt_offset</code>
</li>
<li>
<b>Field added. </b>
<code>u16 cpufeature</code>
</li>
<li>
<b>Field added. </b>
<code>u8 orig_len</code>
</li>
<li>
<b>Field added. </b>
<code>u8 alt_len</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 instr_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 repl_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 cpuid</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 instrlen</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 replacementlen</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 padlen</code>
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

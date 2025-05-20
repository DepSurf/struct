# Struct: <code>text_poke_loc</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct text_poke_loc {
    void *detour;
    void *addr;
    size_t len;
    const const char[5] opcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct text_poke_loc {
    void *detour;
    void *addr;
    size_t len;
    const const char[5] opcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 rel32;
    u8 opcode;
    const const u8[5] text;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 rel32;
    u8 opcode;
    const const u8[5] text;
    u8 old;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 rel32;
    u8 opcode;
    const const u8[5] text;
    u8 old;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 rel32;
    u8 opcode;
    const const u8[5] text;
    u8 old;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 disp;
    u8 len;
    u8 opcode;
    const const u8[5] text;
    u8 old;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 disp;
    u8 len;
    u8 opcode;
    const const u8[5] text;
    u8 old;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 disp;
    u8 len;
    u8 opcode;
    const const u8[5] text;
    u8 old;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct text_poke_loc {
    s32 rel_addr;
    s32 disp;
    u8 len;
    u8 opcode;
    const const u8[5] text;
    u8 old;
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
struct text_poke_loc {
    void *detour;
    void *addr;
    size_t len;
    const const char[5] opcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct text_poke_loc {
    void *detour;
    void *addr;
    size_t len;
    const const char[5] opcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct text_poke_loc {
    void *detour;
    void *addr;
    size_t len;
    const const char[5] opcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct text_poke_loc {
    void *detour;
    void *addr;
    size_t len;
    const const char[5] opcode;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s32 rel_addr</code>
</li>
<li>
<b>Field added. </b>
<code>s32 rel32</code>
</li>
<li>
<b>Field added. </b>
<code>const const u8[5] text</code>
</li>
<li>
<b>Field removed. </b>
<code>void *detour</code>
</li>
<li>
<b>Field removed. </b>
<code>void *addr</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t len</code>
</li>
<li>
<b>Field type changed. </b>
<code>const const char[5] opcode</code> ➡️ <code>u8 opcode</code>
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
<code>u8 old</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s32 disp</code>
</li>
<li>
<b>Field added. </b>
<code>u8 len</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 rel32</code>
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

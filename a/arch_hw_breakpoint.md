# Struct: <code>arch_hw_breakpoint</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
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
struct arch_hw_breakpoint {
    u64 address;
    u64 trigger;
    struct arch_hw_breakpoint_ctrl ctrl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    u32 address;
    u32 trigger;
    struct arch_hw_breakpoint_ctrl step_ctrl;
    struct arch_hw_breakpoint_ctrl ctrl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    u16 type;
    u16 len;
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
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct arch_hw_breakpoint {
    long unsigned int address;
    long unsigned int mask;
    u8 len;
    u8 type;
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
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 trigger</code>
</li>
<li>
<b>Field added. </b>
<code>struct arch_hw_breakpoint_ctrl ctrl</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 len</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 type</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int address</code> ➡️ <code>u64 address</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 trigger</code>
</li>
<li>
<b>Field added. </b>
<code>struct arch_hw_breakpoint_ctrl step_ctrl</code>
</li>
<li>
<b>Field added. </b>
<code>struct arch_hw_breakpoint_ctrl ctrl</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 len</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 type</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int address</code> ➡️ <code>u32 address</code>
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
<code>long unsigned int mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 len</code> ➡️ <code>u16 len</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 type</code> ➡️ <code>u16 type</code>
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

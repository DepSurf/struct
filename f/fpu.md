# Struct: <code>fpu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char fpstate_active;
    unsigned char fpregs_active;
    unsigned char counter;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char fpstate_active;
    unsigned char fpregs_active;
    unsigned char counter;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char fpstate_active;
    unsigned char fpregs_active;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char fpstate_active;
    unsigned char fpregs_active;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char initialized;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char initialized;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    unsigned char initialized;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    struct fpstate *fpstate;
    struct fpstate *__task_fpstate;
    struct fpu_state_perm perm;
    struct fpu_state_perm guest_perm;
    struct fpstate __fpstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    struct fpstate *fpstate;
    struct fpstate *__task_fpstate;
    struct fpu_state_perm perm;
    struct fpu_state_perm guest_perm;
    struct fpstate __fpstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    struct fpstate *fpstate;
    struct fpstate *__task_fpstate;
    struct fpu_state_perm perm;
    struct fpu_state_perm guest_perm;
    struct fpstate __fpstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    struct fpstate *fpstate;
    struct fpstate *__task_fpstate;
    struct fpu_state_perm perm;
    struct fpu_state_perm guest_perm;
    struct fpstate __fpstate;
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
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fpu {
    unsigned int last_cpu;
    long unsigned int avx512_timestamp;
    union fpregs_state state;
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
<b>Field removed. </b>
<code>unsigned char counter</code>
</li>
</ul>
</details>
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
<code>unsigned char initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char fpstate_active</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char fpregs_active</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int avx512_timestamp</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char initialized</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>struct fpstate *fpstate</code>
</li>
<li>
<b>Field added. </b>
<code>struct fpstate *__task_fpstate</code>
</li>
<li>
<b>Field added. </b>
<code>struct fpu_state_perm perm</code>
</li>
<li>
<b>Field added. </b>
<code>struct fpu_state_perm guest_perm</code>
</li>
<li>
<b>Field added. </b>
<code>struct fpstate __fpstate</code>
</li>
<li>
<b>Field removed. </b>
<code>union fpregs_state state</code>
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

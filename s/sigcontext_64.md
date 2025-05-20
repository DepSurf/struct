# Struct: <code>sigcontext_64</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 __pad0;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
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
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sigcontext_64 {
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 di;
    __u64 si;
    __u64 bp;
    __u64 bx;
    __u64 dx;
    __u64 ax;
    __u64 cx;
    __u64 sp;
    __u64 ip;
    __u64 flags;
    __u16 cs;
    __u16 gs;
    __u16 fs;
    __u16 ss;
    __u64 err;
    __u64 trapno;
    __u64 oldmask;
    __u64 cr2;
    __u64 fpstate;
    __u64 reserved1[8];
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
<code>__u16 ss</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 __pad0</code>
</li>
</ul>
</details>
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

# Struct: <code>x86_hw_tss</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
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
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct x86_hw_tss {
    u32 reserved1;
    u64 sp0;
    u64 sp1;
    u64 sp2;
    u64 reserved2;
    u64 ist[7];
    u32 reserved3;
    u32 reserved4;
    u16 reserved5;
    u16 io_bitmap_base;
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

# Struct: <code>sgx_secs</code>

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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sgx_secs {
    u64 size;
    u64 base;
    u32 ssa_frame_size;
    u32 miscselect;
    u8 reserved1[24];
    u64 attributes;
    u64 xfrm;
    u32 mrenclave[8];
    u8 reserved2[32];
    u32 mrsigner[8];
    u8 reserved3[32];
    u32 config_id[16];
    u16 isv_prod_id;
    u16 isv_svn;
    u16 config_svn;
    u8 reserved4[3834];
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

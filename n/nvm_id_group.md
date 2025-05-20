# Struct: <code>nvm_id_group</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvm_id_group {
    u8 mtype;
    u8 fmtype;
    u8 num_ch;
    u8 num_lun;
    u8 num_pln;
    u16 num_blk;
    u16 num_pg;
    u16 fpg_sz;
    u16 csecs;
    u16 sos;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    u32 mpos;
    u32 mccap;
    u16 cpar;
    struct nvm_id_lp_tbl lptbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvm_id_group {
    u8 mtype;
    u8 fmtype;
    u8 num_ch;
    u8 num_lun;
    u8 num_pln;
    u16 num_blk;
    u16 num_pg;
    u16 fpg_sz;
    u16 csecs;
    u16 sos;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    u32 mpos;
    u32 mccap;
    u16 cpar;
    struct nvm_id_lp_tbl lptbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvm_id_group {
    u8 mtype;
    u8 fmtype;
    u8 num_ch;
    u8 num_lun;
    u8 num_pln;
    u16 num_blk;
    u16 num_pg;
    u16 fpg_sz;
    u16 csecs;
    u16 sos;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    u32 mpos;
    u32 mccap;
    u16 cpar;
    struct nvm_id_lp_tbl lptbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvm_id_group {
    u8 mtype;
    u8 fmtype;
    u8 num_ch;
    u8 num_lun;
    u8 num_pln;
    u16 num_blk;
    u16 num_pg;
    u16 fpg_sz;
    u16 csecs;
    u16 sos;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    u32 mpos;
    u32 mccap;
    u16 cpar;
    struct nvm_id_lp_tbl lptbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvm_id_group {
    u8 mtype;
    u8 fmtype;
    u8 num_ch;
    u8 num_lun;
    u8 num_pln;
    u16 num_blk;
    u16 num_pg;
    u16 fpg_sz;
    u16 csecs;
    u16 sos;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    u32 mpos;
    u32 mccap;
    u16 cpar;
    struct nvm_id_lp_tbl lptbl;
};
```
</details>
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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
</ul>

# Struct: <code>nvm_geo</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvm_geo {
    int nr_chnls;
    int nr_luns;
    int luns_per_chnl;
    int nr_planes;
    int sec_per_pg;
    int pgs_per_blk;
    int blks_per_lun;
    int fpg_size;
    int pfpg_size;
    int sec_size;
    int oob_size;
    int mccap;
    struct nvm_addr_format ppaf;
    int max_rq_size;
    int plane_mode;
    int sec_per_pl;
    int sec_per_blk;
    int sec_per_lun;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvm_geo {
    int nr_chnls;
    int nr_luns;
    int luns_per_chnl;
    int nr_planes;
    int sec_per_pg;
    int pgs_per_blk;
    int blks_per_lun;
    int fpg_size;
    int pfpg_size;
    int sec_size;
    int oob_size;
    int mccap;
    struct nvm_addr_format ppaf;
    int max_rq_size;
    int plane_mode;
    int sec_per_pl;
    int sec_per_blk;
    int sec_per_lun;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvm_geo {
    int nr_chnls;
    int nr_luns;
    int luns_per_chnl;
    int nr_planes;
    int sec_per_pg;
    int pgs_per_blk;
    int blks_per_lun;
    int fpg_size;
    int pfpg_size;
    int sec_size;
    int oob_size;
    int mccap;
    struct nvm_addr_format ppaf;
    int max_rq_size;
    int plane_mode;
    int sec_per_pl;
    int sec_per_blk;
    int sec_per_lun;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvm_geo {
    u8 major_ver_id;
    u8 minor_ver_id;
    u8 version;
    int num_ch;
    int num_lun;
    int all_luns;
    int all_chunks;
    int op;
    sector_t total_secs;
    u32 num_chk;
    u32 clba;
    u16 csecs;
    u16 sos;
    bool ext;
    u32 mdts;
    u32 ws_min;
    u32 ws_opt;
    u32 mw_cunits;
    u32 maxoc;
    u32 maxocpu;
    u32 mccap;
    u32 trdt;
    u32 trdm;
    u32 tprt;
    u32 tprm;
    u32 tbet;
    u32 tbem;
    struct nvm_addrf addrf;
    u8 vmnt;
    u32 cap;
    u32 dom;
    u8 mtype;
    u8 fmtype;
    u16 cpar;
    u32 mpos;
    u8 num_pln;
    u8 pln_mode;
    u16 num_pg;
    u16 fpg_sz;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 major_ver_id</code>
</li>
<li>
<b>Field added. </b>
<code>u8 minor_ver_id</code>
</li>
<li>
<b>Field added. </b>
<code>u8 version</code>
</li>
<li>
<b>Field added. </b>
<code>int num_ch</code>
</li>
<li>
<b>Field added. </b>
<code>int num_lun</code>
</li>
<li>
<b>Field added. </b>
<code>int all_luns</code>
</li>
<li>
<b>Field added. </b>
<code>int all_chunks</code>
</li>
<li>
<b>Field added. </b>
<code>int op</code>
</li>
<li>
<b>Field added. </b>
<code>sector_t total_secs</code>
</li>
<li>
<b>Field added. </b>
<code>u32 num_chk</code>
</li>
<li>
<b>Field added. </b>
<code>u32 clba</code>
</li>
<li>
<b>Field added. </b>
<code>u16 csecs</code>
</li>
<li>
<b>Field added. </b>
<code>u16 sos</code>
</li>
<li>
<b>Field added. </b>
<code>u32 ws_min</code>
</li>
<li>
<b>Field added. </b>
<code>u32 ws_opt</code>
</li>
<li>
<b>Field added. </b>
<code>u32 mw_cunits</code>
</li>
<li>
<b>Field added. </b>
<code>u32 maxoc</code>
</li>
<li>
<b>Field added. </b>
<code>u32 maxocpu</code>
</li>
<li>
<b>Field added. </b>
<code>u32 trdt</code>
</li>
<li>
<b>Field added. </b>
<code>u32 trdm</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tprt</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tprm</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tbet</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tbem</code>
</li>
<li>
<b>Field added. </b>
<code>struct nvm_addrf addrf</code>
</li>
<li>
<b>Field added. </b>
<code>u8 vmnt</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cap</code>
</li>
<li>
<b>Field added. </b>
<code>u32 dom</code>
</li>
<li>
<b>Field added. </b>
<code>u8 mtype</code>
</li>
<li>
<b>Field added. </b>
<code>u8 fmtype</code>
</li>
<li>
<b>Field added. </b>
<code>u16 cpar</code>
</li>
<li>
<b>Field added. </b>
<code>u32 mpos</code>
</li>
<li>
<b>Field added. </b>
<code>u8 num_pln</code>
</li>
<li>
<b>Field added. </b>
<code>u8 pln_mode</code>
</li>
<li>
<b>Field added. </b>
<code>u16 num_pg</code>
</li>
<li>
<b>Field added. </b>
<code>u16 fpg_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>int nr_chnls</code>
</li>
<li>
<b>Field removed. </b>
<code>int nr_luns</code>
</li>
<li>
<b>Field removed. </b>
<code>int luns_per_chnl</code>
</li>
<li>
<b>Field removed. </b>
<code>int nr_planes</code>
</li>
<li>
<b>Field removed. </b>
<code>int sec_per_pg</code>
</li>
<li>
<b>Field removed. </b>
<code>int pgs_per_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>int blks_per_lun</code>
</li>
<li>
<b>Field removed. </b>
<code>int fpg_size</code>
</li>
<li>
<b>Field removed. </b>
<code>int pfpg_size</code>
</li>
<li>
<b>Field removed. </b>
<code>int sec_size</code>
</li>
<li>
<b>Field removed. </b>
<code>int oob_size</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nvm_addr_format ppaf</code>
</li>
<li>
<b>Field removed. </b>
<code>int max_rq_size</code>
</li>
<li>
<b>Field removed. </b>
<code>int plane_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>int sec_per_pl</code>
</li>
<li>
<b>Field removed. </b>
<code>int sec_per_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>int sec_per_lun</code>
</li>
<li>
<b>Field type changed. </b>
<code>int mccap</code> ➡️ <code>u32 mccap</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool ext</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 mdts</code>
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
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

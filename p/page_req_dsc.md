# Struct: <code>page_req_dsc</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 srr;
    u64 bof;
    u64 pasid_present;
    u64 lpig;
    u64 pasid;
    u64 bus;
    u64 private;
    u64 prg_index;
    u64 rd_req;
    u64 wr_req;
    u64 exe_req;
    u64 priv_req;
    u64 devfn;
    u64 addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
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
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct page_req_dsc {
    u64 type;
    u64 pasid_present;
    u64 priv_data_present;
    u64 rsvd;
    u64 rid;
    u64 pasid;
    u64 exe_req;
    u64 pm_req;
    u64 rsvd2;
    u64 qw_0;
    u64 rd_req;
    u64 wr_req;
    u64 lpig;
    u64 prg_index;
    u64 addr;
    u64 qw_1;
    u64 priv_data[2];
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 type</code>
</li>
<li>
<b>Field added. </b>
<code>u64 priv_data_present</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rsvd</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rid</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pm_req</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rsvd2</code>
</li>
<li>
<b>Field added. </b>
<code>u64 qw_0</code>
</li>
<li>
<b>Field added. </b>
<code>u64 qw_1</code>
</li>
<li>
<b>Field added. </b>
<code>u64 priv_data[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 srr</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 bof</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 bus</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 private</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 priv_req</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 devfn</code>
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

# Struct: <code>mmc_csd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int tacc_clks;
    unsigned int tacc_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int tacc_clks;
    unsigned int tacc_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int tacc_clks;
    unsigned int tacc_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int tacc_clks;
    unsigned int tacc_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int wp_grp_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
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
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
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
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
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
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmc_csd {
    unsigned char structure;
    unsigned char mmca_vsn;
    short unsigned int cmdclass;
    short unsigned int taac_clks;
    unsigned int taac_ns;
    unsigned int c_size;
    unsigned int r2w_factor;
    unsigned int max_dtr;
    unsigned int erase_size;
    unsigned int read_blkbits;
    unsigned int write_blkbits;
    unsigned int capacity;
    unsigned int read_partial;
    unsigned int read_misalign;
    unsigned int write_partial;
    unsigned int write_misalign;
    unsigned int dsr_imp;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>short unsigned int taac_clks</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int taac_ns</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int tacc_clks</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int tacc_ns</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int wp_grp_size</code>
</li>
</ul>
</details>
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

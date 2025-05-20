# Struct: <code>scsi_eh_save</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    struct request *next_rq;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char cmnd[32];
    struct scsi_data_buffer sdb;
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char cmnd[32];
    struct scsi_data_buffer sdb;
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char cmnd[32];
    struct scsi_data_buffer sdb;
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char cmnd[32];
    struct scsi_data_buffer sdb;
    struct scatterlist sense_sgl;
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
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
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
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct scsi_eh_save {
    int result;
    unsigned int resid_len;
    int eh_eflags;
    enum dma_data_direction data_direction;
    unsigned int underflow;
    unsigned char cmd_len;
    unsigned char prot_op;
    unsigned char *cmnd;
    struct scsi_data_buffer sdb;
    unsigned char eh_cmnd[16];
    struct scatterlist sense_sgl;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int eh_eflags</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>struct request *next_rq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int resid_len</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>unsigned char eh_cmnd[16]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char *cmnd</code> ➡️ <code>unsigned char cmnd[32]</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

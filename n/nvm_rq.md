# Struct: <code>nvm_rq</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_instance *ins;
    struct nvm_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *metadata;
    dma_addr_t dma_metadata;
    struct completion *wait;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_pages;
    uint16_t flags;
    int error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_instance *ins;
    struct nvm_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    struct completion *wait;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_instance *ins;
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    struct completion *wait;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    struct completion *wait;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    struct completion *wait;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
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
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
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
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
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
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvm_rq {
    struct nvm_tgt_dev *dev;
    struct bio *bio;
    struct ppa_addr ppa_addr;
    dma_addr_t dma_ppa_list;
    struct ppa_addr *ppa_list;
    void *meta_list;
    dma_addr_t dma_meta_list;
    nvm_end_io_fn *end_io;
    uint8_t opcode;
    uint16_t nr_ppas;
    uint16_t flags;
    u64 ppa_status;
    int error;
    int is_seq;
    void *private;
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
<code>void *meta_list</code>
</li>
<li>
<b>Field added. </b>
<code>dma_addr_t dma_meta_list</code>
</li>
<li>
<b>Field added. </b>
<code>uint16_t nr_ppas</code>
</li>
<li>
<b>Field added. </b>
<code>u64 ppa_status</code>
</li>
<li>
<b>Field removed. </b>
<code>void *metadata</code>
</li>
<li>
<b>Field removed. </b>
<code>dma_addr_t dma_metadata</code>
</li>
<li>
<b>Field removed. </b>
<code>uint16_t nr_pages</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct nvm_dev *dev</code> ➡️ <code>struct nvm_tgt_dev *dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *private</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nvm_tgt_instance *ins</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct completion *wait</code>
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
<code>int is_seq</code>
</li>
</ul>
</details>
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

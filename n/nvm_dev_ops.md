# Struct: <code>nvm_dev_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_get_l2p_tbl_fn *get_l2p_tbl;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_submit_io_fn *submit_io;
    nvm_erase_blk_fn *erase_block;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
    unsigned int max_phys_sect;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_get_l2p_tbl_fn *get_l2p_tbl;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_submit_io_fn *submit_io;
    nvm_erase_blk_fn *erase_block;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
    unsigned int max_phys_sect;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_get_l2p_tbl_fn *get_l2p_tbl;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_submit_io_fn *submit_io;
    nvm_erase_blk_fn *erase_block;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
    unsigned int max_phys_sect;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_get_l2p_tbl_fn *get_l2p_tbl;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
    unsigned int max_phys_sect;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_get_l2p_tbl_fn *get_l2p_tbl;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_submit_io_fn *submit_io;
    nvm_submit_io_sync_fn *submit_io_sync;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
    unsigned int max_phys_sect;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_submit_io_sync_fn *submit_io_sync;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_submit_io_sync_fn *submit_io_sync;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_submit_io_sync_fn *submit_io_sync;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
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
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
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
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
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
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvm_dev_ops {
    nvm_id_fn *identity;
    nvm_op_bb_tbl_fn *get_bb_tbl;
    nvm_op_set_bb_fn *set_bb_tbl;
    nvm_get_chk_meta_fn *get_chk_meta;
    nvm_submit_io_fn *submit_io;
    nvm_create_dma_pool_fn *create_dma_pool;
    nvm_destroy_dma_pool_fn *destroy_dma_pool;
    nvm_dev_dma_alloc_fn *dev_dma_alloc;
    nvm_dev_dma_free_fn *dev_dma_free;
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
<b>Field removed. </b>
<code>nvm_erase_blk_fn *erase_block</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>nvm_submit_io_sync_fn *submit_io_sync</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>nvm_get_chk_meta_fn *get_chk_meta</code>
</li>
<li>
<b>Field removed. </b>
<code>nvm_get_l2p_tbl_fn *get_l2p_tbl</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int max_phys_sect</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>nvm_submit_io_sync_fn *submit_io_sync</code>
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

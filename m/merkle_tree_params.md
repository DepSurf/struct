# Struct: <code>merkle_tree_params</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct merkle_tree_params {
    struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int level0_blocks;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct merkle_tree_params {
    struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int level0_blocks;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct merkle_tree_params {
    struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int level0_blocks;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct merkle_tree_params {
    struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int level0_blocks;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct merkle_tree_params {
    struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int level0_blocks;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct merkle_tree_params {
    struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int level0_blocks;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int blocks_per_page;
    u8 log_digestsize;
    u8 log_blocksize;
    u8 log_arity;
    u8 log_blocks_per_page;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int tree_pages;
    long unsigned int level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int blocks_per_page;
    u8 log_digestsize;
    u8 log_blocksize;
    u8 log_arity;
    u8 log_blocks_per_page;
    unsigned int num_levels;
    u64 tree_size;
    long unsigned int tree_pages;
    long unsigned int level_start[8];
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
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
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
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct merkle_tree_params {
    const struct fsverity_hash_alg *hash_alg;
    const u8 *hashstate;
    unsigned int digest_size;
    unsigned int block_size;
    unsigned int hashes_per_block;
    unsigned int log_blocksize;
    unsigned int log_arity;
    unsigned int num_levels;
    u64 tree_size;
    u64 level_start[8];
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
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int level0_blocks</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct fsverity_hash_alg *hash_alg</code> ➡️ <code>struct fsverity_hash_alg *hash_alg</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int blocks_per_page</code>
</li>
<li>
<b>Field added. </b>
<code>u8 log_digestsize</code>
</li>
<li>
<b>Field added. </b>
<code>u8 log_blocks_per_page</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int tree_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int level0_blocks</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fsverity_hash_alg *hash_alg</code> ➡️ <code>const struct fsverity_hash_alg *hash_alg</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int log_blocksize</code> ➡️ <code>u8 log_blocksize</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int log_arity</code> ➡️ <code>u8 log_arity</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 level_start[8]</code> ➡️ <code>long unsigned int level_start[8]</code>
</li>
</ul>
</details>
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

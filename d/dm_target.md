# Struct: <code>dm_target</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_write_same_bios;
    unsigned int per_bio_data_size;
    dm_num_write_bios_fn num_write_bios;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
    bool discard_zeroes_data_unsupported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_write_same_bios;
    unsigned int per_io_data_size;
    dm_num_write_bios_fn num_write_bios;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
    bool discard_zeroes_data_unsupported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_write_same_bios;
    unsigned int per_io_data_size;
    dm_num_write_bios_fn num_write_bios;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
    bool discard_zeroes_data_unsupported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    dm_num_write_bios_fn num_write_bios;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    dm_num_write_bios_fn num_write_bios;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool split_discard_bios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool limit_swap_bios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool limit_swap_bios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool limit_swap_bios;
    bool emulate_zone_append;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool limit_swap_bios;
    bool emulate_zone_append;
    bool accounts_remapped_io;
    bool needs_bio_set_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool limit_swap_bios;
    bool emulate_zone_append;
    bool accounts_remapped_io;
    bool needs_bio_set_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool max_discard_granularity;
    bool max_secure_erase_granularity;
    bool max_write_zeroes_granularity;
    bool limit_swap_bios;
    bool emulate_zone_append;
    bool accounts_remapped_io;
    bool needs_bio_set_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
    bool max_discard_granularity;
    bool max_secure_erase_granularity;
    bool max_write_zeroes_granularity;
    bool limit_swap_bios;
    bool emulate_zone_append;
    bool accounts_remapped_io;
    bool needs_bio_set_dev;
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
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
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
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dm_target {
    struct dm_table *table;
    struct target_type *type;
    sector_t begin;
    sector_t len;
    uint32_t max_io_len;
    unsigned int num_flush_bios;
    unsigned int num_discard_bios;
    unsigned int num_secure_erase_bios;
    unsigned int num_write_same_bios;
    unsigned int num_write_zeroes_bios;
    unsigned int per_io_data_size;
    void *private;
    char *error;
    bool flush_supported;
    bool discards_supported;
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
<code>unsigned int per_io_data_size</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int per_bio_data_size</code>
</li>
</ul>
</details>
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
<code>unsigned int num_write_zeroes_bios</code>
</li>
<li>
<b>Field removed. </b>
<code>bool discard_zeroes_data_unsupported</code>
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
<b>Field added. </b>
<code>unsigned int num_secure_erase_bios</code>
</li>
<li>
<b>Field removed. </b>
<code>dm_num_write_bios_fn num_write_bios</code>
</li>
</ul>
</details>
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
<code>bool split_discard_bios</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool limit_swap_bios</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool emulate_zone_append</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool accounts_remapped_io</code>
</li>
<li>
<b>Field added. </b>
<code>bool needs_bio_set_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int num_write_same_bios</code>
</li>
</ul>
</details>
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
<code>bool max_discard_granularity</code>
</li>
<li>
<b>Field added. </b>
<code>bool max_secure_erase_granularity</code>
</li>
<li>
<b>Field added. </b>
<code>bool max_write_zeroes_granularity</code>
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

# Struct: <code>ext4_fs_context</code>

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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ext4_fs_context {
    char * s_qf_names[3];
    struct fscrypt_dummy_policy dummy_enc_policy;
    int s_jquota_fmt;
    short unsigned int qname_spec;
    long unsigned int vals_s_flags;
    long unsigned int mask_s_flags;
    long unsigned int journal_devnum;
    long unsigned int s_commit_interval;
    long unsigned int s_stripe;
    unsigned int s_inode_readahead_blks;
    unsigned int s_want_extra_isize;
    unsigned int s_li_wait_mult;
    unsigned int s_max_dir_size_kb;
    unsigned int journal_ioprio;
    unsigned int vals_s_mount_opt;
    unsigned int mask_s_mount_opt;
    unsigned int vals_s_mount_opt2;
    unsigned int mask_s_mount_opt2;
    long unsigned int vals_s_mount_flags;
    long unsigned int mask_s_mount_flags;
    unsigned int opt_flags;
    unsigned int spec;
    u32 s_max_batch_time;
    u32 s_min_batch_time;
    kuid_t s_resuid;
    kgid_t s_resgid;
    ext4_fsblk_t s_sb_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ext4_fs_context {
    char * s_qf_names[3];
    struct fscrypt_dummy_policy dummy_enc_policy;
    int s_jquota_fmt;
    short unsigned int qname_spec;
    long unsigned int vals_s_flags;
    long unsigned int mask_s_flags;
    long unsigned int journal_devnum;
    long unsigned int s_commit_interval;
    long unsigned int s_stripe;
    unsigned int s_inode_readahead_blks;
    unsigned int s_want_extra_isize;
    unsigned int s_li_wait_mult;
    unsigned int s_max_dir_size_kb;
    unsigned int journal_ioprio;
    unsigned int vals_s_mount_opt;
    unsigned int mask_s_mount_opt;
    unsigned int vals_s_mount_opt2;
    unsigned int mask_s_mount_opt2;
    long unsigned int vals_s_mount_flags;
    long unsigned int mask_s_mount_flags;
    unsigned int opt_flags;
    unsigned int spec;
    u32 s_max_batch_time;
    u32 s_min_batch_time;
    kuid_t s_resuid;
    kgid_t s_resgid;
    ext4_fsblk_t s_sb_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ext4_fs_context {
    char * s_qf_names[3];
    struct fscrypt_dummy_policy dummy_enc_policy;
    int s_jquota_fmt;
    short unsigned int qname_spec;
    long unsigned int vals_s_flags;
    long unsigned int mask_s_flags;
    long unsigned int journal_devnum;
    long unsigned int s_commit_interval;
    long unsigned int s_stripe;
    unsigned int s_inode_readahead_blks;
    unsigned int s_want_extra_isize;
    unsigned int s_li_wait_mult;
    unsigned int s_max_dir_size_kb;
    unsigned int journal_ioprio;
    unsigned int vals_s_mount_opt;
    unsigned int mask_s_mount_opt;
    unsigned int vals_s_mount_opt2;
    unsigned int mask_s_mount_opt2;
    long unsigned int vals_s_mount_flags;
    long unsigned int mask_s_mount_flags;
    unsigned int opt_flags;
    unsigned int spec;
    u32 s_max_batch_time;
    u32 s_min_batch_time;
    kuid_t s_resuid;
    kgid_t s_resgid;
    ext4_fsblk_t s_sb_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ext4_fs_context {
    char * s_qf_names[3];
    struct fscrypt_dummy_policy dummy_enc_policy;
    int s_jquota_fmt;
    short unsigned int qname_spec;
    long unsigned int vals_s_flags;
    long unsigned int mask_s_flags;
    long unsigned int journal_devnum;
    long unsigned int s_commit_interval;
    long unsigned int s_stripe;
    unsigned int s_inode_readahead_blks;
    unsigned int s_want_extra_isize;
    unsigned int s_li_wait_mult;
    unsigned int s_max_dir_size_kb;
    unsigned int journal_ioprio;
    unsigned int vals_s_mount_opt;
    unsigned int mask_s_mount_opt;
    unsigned int vals_s_mount_opt2;
    unsigned int mask_s_mount_opt2;
    unsigned int opt_flags;
    unsigned int spec;
    u32 s_max_batch_time;
    u32 s_min_batch_time;
    kuid_t s_resuid;
    kgid_t s_resgid;
    ext4_fsblk_t s_sb_block;
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
<b>Field removed. </b>
<code>long unsigned int vals_s_mount_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mask_s_mount_flags</code>
</li>
</ul>
</details>
</li>
</ul>

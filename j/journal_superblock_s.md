# Struct: <code>journal_superblock_s</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __u32 s_padding[41];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __u32 s_padding[41];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __u32 s_padding[41];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __u32 s_padding[41];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __u32 s_padding[41];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __be32 s_head;
    __u32 s_padding[40];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __be32 s_num_fc_blks;
    __be32 s_head;
    __u32 s_padding[40];
    __be32 s_checksum;
    __u8 s_users[768];
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
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
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
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct journal_superblock_s {
    journal_header_t s_header;
    __be32 s_blocksize;
    __be32 s_maxlen;
    __be32 s_first;
    __be32 s_sequence;
    __be32 s_start;
    __be32 s_errno;
    __be32 s_feature_compat;
    __be32 s_feature_incompat;
    __be32 s_feature_ro_compat;
    __u8 s_uuid[16];
    __be32 s_nr_users;
    __be32 s_dynsuper;
    __be32 s_max_transaction;
    __be32 s_max_trans_data;
    __u8 s_checksum_type;
    __u8 s_padding2[3];
    __u32 s_padding[42];
    __be32 s_checksum;
    __u8 s_users[768];
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
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
<code>__be32 s_num_fc_blks</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 s_padding[42]</code> ➡️ <code>__u32 s_padding[41]</code>
</li>
</ul>
</details>
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
<code>__be32 s_head</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 s_padding[41]</code> ➡️ <code>__u32 s_padding[40]</code>
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

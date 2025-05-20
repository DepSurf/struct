# Struct: <code>ext4_super_block</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __le32 s_reserved[98];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __le32 s_reserved[98];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __le32 s_reserved[98];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __le32 s_reserved[98];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __le32 s_reserved[98];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __le32 s_reserved[98];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le32 s_reserved[96];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_orphan_file_inum;
    __le32 s_reserved[94];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_orphan_file_inum;
    __le32 s_reserved[94];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_orphan_file_inum;
    __le32 s_reserved[94];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_orphan_file_inum;
    __le32 s_reserved[94];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_first_error_errcode;
    __u8 s_last_error_errcode;
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_orphan_file_inum;
    __le32 s_reserved[94];
    __le32 s_checksum;
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
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
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
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ext4_super_block {
    __le32 s_inodes_count;
    __le32 s_blocks_count_lo;
    __le32 s_r_blocks_count_lo;
    __le32 s_free_blocks_count_lo;
    __le32 s_free_inodes_count;
    __le32 s_first_data_block;
    __le32 s_log_block_size;
    __le32 s_log_cluster_size;
    __le32 s_blocks_per_group;
    __le32 s_clusters_per_group;
    __le32 s_inodes_per_group;
    __le32 s_mtime;
    __le32 s_wtime;
    __le16 s_mnt_count;
    __le16 s_max_mnt_count;
    __le16 s_magic;
    __le16 s_state;
    __le16 s_errors;
    __le16 s_minor_rev_level;
    __le32 s_lastcheck;
    __le32 s_checkinterval;
    __le32 s_creator_os;
    __le32 s_rev_level;
    __le16 s_def_resuid;
    __le16 s_def_resgid;
    __le32 s_first_ino;
    __le16 s_inode_size;
    __le16 s_block_group_nr;
    __le32 s_feature_compat;
    __le32 s_feature_incompat;
    __le32 s_feature_ro_compat;
    __u8 s_uuid[16];
    char s_volume_name[16];
    char s_last_mounted[64];
    __le32 s_algorithm_usage_bitmap;
    __u8 s_prealloc_blocks;
    __u8 s_prealloc_dir_blocks;
    __le16 s_reserved_gdt_blocks;
    __u8 s_journal_uuid[16];
    __le32 s_journal_inum;
    __le32 s_journal_dev;
    __le32 s_last_orphan;
    __le32 s_hash_seed[4];
    __u8 s_def_hash_version;
    __u8 s_jnl_backup_type;
    __le16 s_desc_size;
    __le32 s_default_mount_opts;
    __le32 s_first_meta_bg;
    __le32 s_mkfs_time;
    __le32 s_jnl_blocks[17];
    __le32 s_blocks_count_hi;
    __le32 s_r_blocks_count_hi;
    __le32 s_free_blocks_count_hi;
    __le16 s_min_extra_isize;
    __le16 s_want_extra_isize;
    __le32 s_flags;
    __le16 s_raid_stride;
    __le16 s_mmp_update_interval;
    __le64 s_mmp_block;
    __le32 s_raid_stripe_width;
    __u8 s_log_groups_per_flex;
    __u8 s_checksum_type;
    __u8 s_encryption_level;
    __u8 s_reserved_pad;
    __le64 s_kbytes_written;
    __le32 s_snapshot_inum;
    __le32 s_snapshot_id;
    __le64 s_snapshot_r_blocks_count;
    __le32 s_snapshot_list;
    __le32 s_error_count;
    __le32 s_first_error_time;
    __le32 s_first_error_ino;
    __le64 s_first_error_block;
    __u8 s_first_error_func[32];
    __le32 s_first_error_line;
    __le32 s_last_error_time;
    __le32 s_last_error_ino;
    __le32 s_last_error_line;
    __le64 s_last_error_block;
    __u8 s_last_error_func[32];
    __u8 s_mount_opts[64];
    __le32 s_usr_quota_inum;
    __le32 s_grp_quota_inum;
    __le32 s_overhead_clusters;
    __le32 s_backup_bgs[2];
    __u8 s_encrypt_algos[4];
    __u8 s_encrypt_pw_salt[16];
    __le32 s_lpf_ino;
    __le32 s_prj_quota_inum;
    __le32 s_checksum_seed;
    __u8 s_wtime_hi;
    __u8 s_mtime_hi;
    __u8 s_mkfs_time_hi;
    __u8 s_lastcheck_hi;
    __u8 s_first_error_time_hi;
    __u8 s_last_error_time_hi;
    __u8 s_pad[2];
    __le16 s_encoding;
    __le16 s_encoding_flags;
    __le32 s_reserved[95];
    __le32 s_checksum;
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 s_wtime_hi</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_mtime_hi</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_mkfs_time_hi</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_lastcheck_hi</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_first_error_time_hi</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_last_error_time_hi</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_pad[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>__le32 s_reserved[98]</code> ➡️ <code>__le32 s_reserved[96]</code>
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
<code>__le16 s_encoding</code>
</li>
<li>
<b>Field added. </b>
<code>__le16 s_encoding_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>__le32 s_reserved[96]</code> ➡️ <code>__le32 s_reserved[95]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 s_first_error_errcode</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 s_last_error_errcode</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 s_pad[2]</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__le32 s_orphan_file_inum</code>
</li>
<li>
<b>Field type changed. </b>
<code>__le32 s_reserved[95]</code> ➡️ <code>__le32 s_reserved[94]</code>
</li>
</ul>
</details>
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

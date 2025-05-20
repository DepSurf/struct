# Struct: <code>mdp_superblock_s</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
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
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
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
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mdp_superblock_s {
    __u32 md_magic;
    __u32 major_version;
    __u32 minor_version;
    __u32 patch_version;
    __u32 gvalid_words;
    __u32 set_uuid0;
    __u32 ctime;
    __u32 level;
    __u32 size;
    __u32 nr_disks;
    __u32 raid_disks;
    __u32 md_minor;
    __u32 not_persistent;
    __u32 set_uuid1;
    __u32 set_uuid2;
    __u32 set_uuid3;
    __u32 gstate_creserved[16];
    __u32 utime;
    __u32 state;
    __u32 active_disks;
    __u32 working_disks;
    __u32 failed_disks;
    __u32 spare_disks;
    __u32 sb_csum;
    __u32 events_lo;
    __u32 events_hi;
    __u32 cp_events_lo;
    __u32 cp_events_hi;
    __u32 recovery_cp;
    __u64 reshape_position;
    __u32 new_level;
    __u32 delta_disks;
    __u32 new_layout;
    __u32 new_chunk;
    __u32 gstate_sreserved[14];
    __u32 layout;
    __u32 chunk_size;
    __u32 root_pv;
    __u32 root_block;
    __u32 pstate_reserved[60];
    mdp_disk_t disks[27];
    __u32 reserved[0];
    mdp_disk_t this_disk;
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

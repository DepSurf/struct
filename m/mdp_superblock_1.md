# Struct: <code>mdp_superblock_1</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
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
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
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
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mdp_superblock_1 {
    __le32 magic;
    __le32 major_version;
    __le32 feature_map;
    __le32 pad0;
    __u8 set_uuid[16];
    char set_name[32];
    __le64 ctime;
    __le32 level;
    __le32 layout;
    __le64 size;
    __le32 chunksize;
    __le32 raid_disks;
    __le32 bitmap_offset;
    struct (anon) ppl;
    __le32 new_level;
    __le64 reshape_position;
    __le32 delta_disks;
    __le32 new_layout;
    __le32 new_chunk;
    __le32 new_offset;
    __le64 data_offset;
    __le64 data_size;
    __le64 super_offset;
    __le64 recovery_offset;
    __le64 journal_tail;
    __le32 dev_number;
    __le32 cnt_corrected_read;
    __u8 device_uuid[16];
    __u8 devflags;
    __u8 bblog_shift;
    __le16 bblog_size;
    __le32 bblog_offset;
    __le64 utime;
    __le64 events;
    __le64 resync_offset;
    __le32 sb_csum;
    __le32 max_dev;
    __u8 pad3[32];
    __le16 dev_roles[0];
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
<code>struct (anon) ppl</code>
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

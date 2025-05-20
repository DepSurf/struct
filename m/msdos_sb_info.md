# Struct: <code>msdos_sb_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
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
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
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
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct msdos_sb_info {
    short unsigned int sec_per_clus;
    short unsigned int cluster_bits;
    unsigned int cluster_size;
    unsigned char fats;
    unsigned char fat_bits;
    short unsigned int fat_start;
    long unsigned int fat_length;
    long unsigned int dir_start;
    short unsigned int dir_entries;
    long unsigned int data_start;
    long unsigned int max_cluster;
    long unsigned int root_cluster;
    long unsigned int fsinfo_sector;
    struct mutex fat_lock;
    struct mutex nfs_build_inode_lock;
    struct mutex s_lock;
    unsigned int prev_free;
    unsigned int free_clusters;
    unsigned int free_clus_valid;
    struct fat_mount_options options;
    struct nls_table *nls_disk;
    struct nls_table *nls_io;
    const void *dir_ops;
    int dir_per_block;
    int dir_per_block_bits;
    unsigned int vol_id;
    int fatent_shift;
    const struct fatent_operations *fatent_ops;
    struct inode *fat_inode;
    struct inode *fsinfo_inode;
    struct ratelimit_state ratelimit;
    spinlock_t inode_hash_lock;
    struct hlist_head inode_hashtable[256];
    spinlock_t dir_hash_lock;
    struct hlist_head dir_hashtable[256];
    unsigned int dirty;
    struct callback_head rcu;
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
<b>Field type changed. </b>
<code>struct fatent_operations *fatent_ops</code> ➡️ <code>const struct fatent_operations *fatent_ops</code>
</li>
</ul>
</details>
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

# Struct: <code>fscrypt_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fscrypt_operations {
    int (*get_context)(struct inode *, void *, size_t);
    int (*key_prefix)(struct inode *, u8 **);
    int (*prepare_context)(struct inode *);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    int (*dummy_context)(struct inode *);
    bool (*is_encrypted)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int (*max_namelen)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    int (*get_context)(struct inode *, void *, size_t);
    int (*key_prefix)(struct inode *, u8 **);
    int (*prepare_context)(struct inode *);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    int (*dummy_context)(struct inode *);
    bool (*is_encrypted)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int (*max_namelen)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*is_encrypted)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int (*max_namelen)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int (*max_namelen)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_context * (*get_dummy_context)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
    int (*get_num_devices)(struct super_block *);
    void (*get_devices)(struct super_block *, struct request_queue **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
    int (*get_num_devices)(struct super_block *);
    void (*get_devices)(struct super_block *, struct request_queue **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
    int (*get_num_devices)(struct super_block *);
    void (*get_devices)(struct super_block *, struct request_queue **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
    int (*get_num_devices)(struct super_block *);
    void (*get_devices)(struct super_block *, struct request_queue **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
    struct block_device ** (*get_devices)(struct super_block *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    bool (*has_stable_inodes)(struct super_block *);
    void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *);
    struct block_device ** (*get_devices)(struct super_block *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int needs_bounce_pages;
    unsigned int has_32bit_inodes;
    unsigned int supports_subblock_data_units;
    const char *legacy_key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    const union fscrypt_policy * (*get_dummy_policy)(struct super_block *);
    bool (*empty_dir)(struct inode *);
    bool (*has_stable_inodes)(struct super_block *);
    struct block_device ** (*get_devices)(struct super_block *, unsigned int *);
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
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
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
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fscrypt_operations {
    unsigned int flags;
    const char *key_prefix;
    int (*get_context)(struct inode *, void *, size_t);
    int (*set_context)(struct inode *, const void *, size_t, void *);
    bool (*dummy_context)(struct inode *);
    bool (*empty_dir)(struct inode *);
    unsigned int max_namelen;
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*prepare_context)(struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*key_prefix)(struct inode *, u8 **)</code> ➡️ <code>const char *key_prefix</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dummy_context)(struct inode *)</code> ➡️ <code>bool (*dummy_context)(struct inode *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool (*is_encrypted)(struct inode *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int (*max_namelen)(struct inode *)</code> ➡️ <code>unsigned int max_namelen</code>
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const union fscrypt_context * (*get_dummy_context)(struct super_block *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*has_stable_inodes)(struct super_block *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*dummy_context)(struct inode *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const union fscrypt_policy * (*get_dummy_policy)(struct super_block *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_num_devices)(struct super_block *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_devices)(struct super_block *, struct request_queue **)</code>
</li>
<li>
<b>Field removed. </b>
<code>const union fscrypt_context * (*get_dummy_context)(struct super_block *)</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int max_namelen</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*get_num_devices)(struct super_block *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get_devices)(struct super_block *, struct request_queue **)</code> ➡️ <code>struct block_device ** (*get_devices)(struct super_block *, unsigned int *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int needs_bounce_pages</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int has_32bit_inodes</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int supports_subblock_data_units</code>
</li>
<li>
<b>Field added. </b>
<code>const char *legacy_key_prefix</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
</li>
<li>
<b>Field removed. </b>
<code>const char *key_prefix</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*get_ino_and_lblk_bits)(struct super_block *, int *, int *)</code>
</li>
</ul>
</details>
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

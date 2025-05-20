# Struct: <code>integrity_iint_cache</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_module_status;
    enum integrity_status ima_firmware_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    long unsigned int real_ino;
    dev_t real_dev;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
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
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
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
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct integrity_iint_cache {
    struct rb_node rb_node;
    struct mutex mutex;
    struct inode *inode;
    u64 version;
    long unsigned int flags;
    long unsigned int measured_pcrs;
    long unsigned int atomic_flags;
    enum integrity_status ima_file_status;
    enum integrity_status ima_mmap_status;
    enum integrity_status ima_bprm_status;
    enum integrity_status ima_read_status;
    enum integrity_status ima_creds_status;
    enum integrity_status evm_status;
    struct ima_digest_data *ima_hash;
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
<code>long unsigned int measured_pcrs</code>
</li>
<li>
<b>Field added. </b>
<code>enum integrity_status ima_read_status</code>
</li>
<li>
<b>Field removed. </b>
<code>enum integrity_status ima_module_status</code>
</li>
<li>
<b>Field removed. </b>
<code>enum integrity_status ima_firmware_status</code>
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex mutex</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int atomic_flags</code>
</li>
<li>
<b>Field added. </b>
<code>enum integrity_status ima_creds_status</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int real_ino</code>
</li>
<li>
<b>Field added. </b>
<code>dev_t real_dev</code>
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

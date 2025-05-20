# Struct: <code>lsm_blob_sizes</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_ipc;
    int lbs_key;
    int lbs_msg_msg;
    int lbs_sock;
    int lbs_superblock;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_ipc;
    int lbs_key;
    int lbs_msg_msg;
    int lbs_sock;
    int lbs_superblock;
    int lbs_task;
};
```
</details>
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_superblock;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_superblock;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_superblock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_superblock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_superblock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_superblock;
    int lbs_ipc;
    int lbs_key;
    int lbs_msg_msg;
    int lbs_task;
    int lbs_xattr_count;
    int lbs_mnt_opts;
    bool lbs_secmark;
    bool lbs_netlabel;
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
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
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
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct lsm_blob_sizes {
    int lbs_cred;
    int lbs_file;
    int lbs_inode;
    int lbs_sock;
    int lbs_ipc;
    int lbs_msg_msg;
    int lbs_task;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int lbs_superblock</code>
</li>
</ul>
</details>
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
<code>int lbs_key</code>
</li>
<li>
<b>Field added. </b>
<code>int lbs_xattr_count</code>
</li>
<li>
<b>Field added. </b>
<code>int lbs_mnt_opts</code>
</li>
<li>
<b>Field added. </b>
<code>bool lbs_secmark</code>
</li>
<li>
<b>Field added. </b>
<code>bool lbs_netlabel</code>
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

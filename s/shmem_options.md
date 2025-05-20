# Struct: <code>shmem_options</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
    bool noswap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    long long unsigned int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    bool full_inums;
    int huge;
    int seen;
    bool noswap;
    short unsigned int quota_types;
    struct shmem_quota_limits qlimits;
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
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
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
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct shmem_options {
    long long unsigned int blocks;
    int inodes;
    struct mempolicy *mpol;
    kuid_t uid;
    kgid_t gid;
    umode_t mode;
    int huge;
    int seen;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool full_inums</code>
</li>
<li>
<b>Field type changed. </b>
<code>int inodes</code> ➡️ <code>long long unsigned int inodes</code>
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
<code>bool noswap</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>short unsigned int quota_types</code>
</li>
<li>
<b>Field added. </b>
<code>struct shmem_quota_limits qlimits</code>
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

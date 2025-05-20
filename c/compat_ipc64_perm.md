# Struct: <code>compat_ipc64_perm</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    compat_mode_t mode;
    unsigned char __pad1[2];
    compat_ushort_t seq;
    compat_ushort_t __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    compat_mode_t mode;
    unsigned char __pad1[2];
    compat_ushort_t seq;
    compat_ushort_t __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    compat_mode_t mode;
    unsigned char __pad1[2];
    compat_ushort_t seq;
    compat_ushort_t __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    compat_mode_t mode;
    unsigned char __pad1[2];
    compat_ushort_t seq;
    compat_ushort_t __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
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
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid_t uid;
    __compat_gid_t gid;
    __compat_uid_t cuid;
    __compat_gid_t cgid;
    compat_mode_t mode;
    unsigned int seq;
    unsigned int __pad2;
    long unsigned int __unused1;
    long unsigned int __unused2;
};
```
</details>
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct compat_ipc64_perm {
    compat_key_t key;
    __compat_uid32_t uid;
    __compat_gid32_t gid;
    __compat_uid32_t cuid;
    __compat_gid32_t cgid;
    short unsigned int mode;
    short unsigned int __pad1;
    short unsigned int seq;
    short unsigned int __pad2;
    compat_ulong_t unused1;
    compat_ulong_t unused2;
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>short unsigned int mode</code> ➡️ <code>compat_mode_t mode</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int __pad1</code> ➡️ <code>unsigned char __pad1[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int seq</code> ➡️ <code>compat_ushort_t seq</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int __pad2</code> ➡️ <code>compat_ushort_t __pad2</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int __unused1</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int __unused2</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int __pad1</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t unused1</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t unused2</code>
</li>
<li>
<b>Field type changed. </b>
<code>__compat_uid32_t uid</code> ➡️ <code>__compat_uid_t uid</code>
</li>
<li>
<b>Field type changed. </b>
<code>__compat_gid32_t gid</code> ➡️ <code>__compat_gid_t gid</code>
</li>
<li>
<b>Field type changed. </b>
<code>__compat_uid32_t cuid</code> ➡️ <code>__compat_uid_t cuid</code>
</li>
<li>
<b>Field type changed. </b>
<code>__compat_gid32_t cgid</code> ➡️ <code>__compat_gid_t cgid</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int mode</code> ➡️ <code>compat_mode_t mode</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int seq</code> ➡️ <code>unsigned int seq</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int __pad2</code> ➡️ <code>unsigned int __pad2</code>
</li>
</ul>
</details>
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

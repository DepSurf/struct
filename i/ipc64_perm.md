# Struct: <code>ipc64_perm</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
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
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[2];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid_t uid;
    __kernel_gid_t gid;
    __kernel_uid_t cuid;
    __kernel_gid_t cgid;
    __kernel_mode_t mode;
    unsigned int seq;
    unsigned int __pad1;
    long long unsigned int __unused1;
    long long unsigned int __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
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
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ipc64_perm {
    __kernel_key_t key;
    __kernel_uid32_t uid;
    __kernel_gid32_t gid;
    __kernel_uid32_t cuid;
    __kernel_gid32_t cgid;
    __kernel_mode_t mode;
    unsigned char __pad1[0];
    short unsigned int seq;
    short unsigned int __pad2;
    __kernel_ulong_t __unused1;
    __kernel_ulong_t __unused2;
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned char __pad1[0]</code> ➡️ <code>unsigned char __pad1[2]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>short unsigned int __pad2</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_uid32_t uid</code> ➡️ <code>__kernel_uid_t uid</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_gid32_t gid</code> ➡️ <code>__kernel_gid_t gid</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_uid32_t cuid</code> ➡️ <code>__kernel_uid_t cuid</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_gid32_t cgid</code> ➡️ <code>__kernel_gid_t cgid</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char __pad1[0]</code> ➡️ <code>unsigned int __pad1</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int seq</code> ➡️ <code>unsigned int seq</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_ulong_t __unused1</code> ➡️ <code>long long unsigned int __unused1</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_ulong_t __unused2</code> ➡️ <code>long long unsigned int __unused2</code>
</li>
</ul>
</details>
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

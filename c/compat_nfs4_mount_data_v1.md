# Struct: <code>compat_nfs4_mount_data_v1</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
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
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
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
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct compat_nfs4_mount_data_v1 {
    compat_int_t version;
    compat_int_t flags;
    compat_int_t rsize;
    compat_int_t wsize;
    compat_int_t timeo;
    compat_int_t retrans;
    compat_int_t acregmin;
    compat_int_t acregmax;
    compat_int_t acdirmin;
    compat_int_t acdirmax;
    struct compat_nfs_string client_addr;
    struct compat_nfs_string mnt_path;
    struct compat_nfs_string hostname;
    compat_uint_t host_addrlen;
    compat_uptr_t host_addr;
    compat_int_t proto;
    compat_int_t auth_flavourlen;
    compat_uptr_t auth_flavours;
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
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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

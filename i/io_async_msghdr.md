# Struct: <code>io_async_msghdr</code>

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
In <code>5.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec *iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec *iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec *free_iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec *free_iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec *free_iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec fast_iov_one;
    __kernel_size_t controllen;
    int namelen;
    __kernel_size_t payloadlen;
    struct io_cache_entry cache;
    struct iovec *free_iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec fast_iov_one;
    __kernel_size_t controllen;
    int namelen;
    __kernel_size_t payloadlen;
    struct io_cache_entry cache;
    struct iovec *free_iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_async_msghdr {
    struct iovec fast_iov[8];
    struct iovec fast_iov_one;
    __kernel_size_t controllen;
    int namelen;
    __kernel_size_t payloadlen;
    struct io_cache_entry cache;
    struct iovec *free_iov;
    struct sockaddr *uaddr;
    struct msghdr msg;
    struct __kernel_sockaddr_storage addr;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iovec *free_iov</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iovec *iov</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iovec fast_iov_one</code>
</li>
<li>
<b>Field added. </b>
<code>__kernel_size_t controllen</code>
</li>
<li>
<b>Field added. </b>
<code>int namelen</code>
</li>
<li>
<b>Field added. </b>
<code>__kernel_size_t payloadlen</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_cache_entry cache</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

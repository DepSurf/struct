# Struct: <code>mptcp_subflow_addrs</code>

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
In <code>5.8</code>: Absent ⚠️
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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_subflow_addrs {
    __kernel_sa_family_t sa_family;
    struct sockaddr sa_local;
    struct sockaddr_in sin_local;
    struct sockaddr_in6 sin6_local;
    struct __kernel_sockaddr_storage ss_local;
    struct sockaddr sa_remote;
    struct sockaddr_in sin_remote;
    struct sockaddr_in6 sin6_remote;
    struct __kernel_sockaddr_storage ss_remote;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_subflow_addrs {
    __kernel_sa_family_t sa_family;
    struct sockaddr sa_local;
    struct sockaddr_in sin_local;
    struct sockaddr_in6 sin6_local;
    struct __kernel_sockaddr_storage ss_local;
    struct sockaddr sa_remote;
    struct sockaddr_in sin_remote;
    struct sockaddr_in6 sin6_remote;
    struct __kernel_sockaddr_storage ss_remote;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_subflow_addrs {
    __kernel_sa_family_t sa_family;
    struct sockaddr sa_local;
    struct sockaddr_in sin_local;
    struct sockaddr_in6 sin6_local;
    struct __kernel_sockaddr_storage ss_local;
    struct sockaddr sa_remote;
    struct sockaddr_in sin_remote;
    struct sockaddr_in6 sin6_remote;
    struct __kernel_sockaddr_storage ss_remote;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_subflow_addrs {
    __kernel_sa_family_t sa_family;
    struct sockaddr sa_local;
    struct sockaddr_in sin_local;
    struct sockaddr_in6 sin6_local;
    struct __kernel_sockaddr_storage ss_local;
    struct sockaddr sa_remote;
    struct sockaddr_in sin_remote;
    struct sockaddr_in6 sin6_remote;
    struct __kernel_sockaddr_storage ss_remote;
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

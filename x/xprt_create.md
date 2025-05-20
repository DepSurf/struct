# Struct: <code>xprt_create</code>

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
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xprt_create {
    int ident;
    struct net *net;
    struct sockaddr *srcaddr;
    struct sockaddr *dstaddr;
    size_t addrlen;
    const char *servername;
    struct svc_xprt *bc_xprt;
    struct rpc_xprt_switch *bc_xps;
    unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xprt_create {
    int ident;
    struct net *net;
    struct sockaddr *srcaddr;
    struct sockaddr *dstaddr;
    size_t addrlen;
    const char *servername;
    struct svc_xprt *bc_xprt;
    struct rpc_xprt_switch *bc_xps;
    unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xprt_create {
    int ident;
    struct net *net;
    struct sockaddr *srcaddr;
    struct sockaddr *dstaddr;
    size_t addrlen;
    const char *servername;
    struct svc_xprt *bc_xprt;
    struct rpc_xprt_switch *bc_xps;
    unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xprt_create {
    int ident;
    struct net *net;
    struct sockaddr *srcaddr;
    struct sockaddr *dstaddr;
    size_t addrlen;
    const char *servername;
    struct svc_xprt *bc_xprt;
    struct rpc_xprt_switch *bc_xps;
    unsigned int flags;
    struct xprtsec_parms xprtsec;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xprt_create {
    int ident;
    struct net *net;
    struct sockaddr *srcaddr;
    struct sockaddr *dstaddr;
    size_t addrlen;
    const char *servername;
    struct svc_xprt *bc_xprt;
    struct rpc_xprt_switch *bc_xps;
    unsigned int flags;
    struct xprtsec_parms xprtsec;
    long unsigned int connect_timeout;
    long unsigned int reconnect_timeout;
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
<code>struct xprtsec_parms xprtsec</code>
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
<code>long unsigned int connect_timeout</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int reconnect_timeout</code>
</li>
</ul>
</details>
</li>
</ul>

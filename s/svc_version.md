# Struct: <code>svc_version</code>

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
struct svc_version {
    u32 vs_vers;
    u32 vs_nproc;
    const struct svc_procedure *vs_proc;
    unsigned int *vs_count;
    u32 vs_xdrsize;
    bool vs_hidden;
    bool vs_rpcb_optnl;
    bool vs_need_cong_ctrl;
    int (*vs_dispatch)(struct svc_rqst *, __be32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct svc_version {
    u32 vs_vers;
    u32 vs_nproc;
    const struct svc_procedure *vs_proc;
    unsigned int *vs_count;
    u32 vs_xdrsize;
    bool vs_hidden;
    bool vs_rpcb_optnl;
    bool vs_need_cong_ctrl;
    int (*vs_dispatch)(struct svc_rqst *, __be32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct svc_version {
    u32 vs_vers;
    u32 vs_nproc;
    const struct svc_procedure *vs_proc;
    unsigned int *vs_count;
    u32 vs_xdrsize;
    bool vs_hidden;
    bool vs_rpcb_optnl;
    bool vs_need_cong_ctrl;
    int (*vs_dispatch)(struct svc_rqst *, __be32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct svc_version {
    u32 vs_vers;
    u32 vs_nproc;
    const struct svc_procedure *vs_proc;
    long unsigned int *vs_count;
    u32 vs_xdrsize;
    bool vs_hidden;
    bool vs_rpcb_optnl;
    bool vs_need_cong_ctrl;
    int (*vs_dispatch)(struct svc_rqst *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct svc_version {
    u32 vs_vers;
    u32 vs_nproc;
    const struct svc_procedure *vs_proc;
    long unsigned int *vs_count;
    u32 vs_xdrsize;
    bool vs_hidden;
    bool vs_rpcb_optnl;
    bool vs_need_cong_ctrl;
    int (*vs_dispatch)(struct svc_rqst *);
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
<b>Field type changed. </b>
<code>unsigned int *vs_count</code> ➡️ <code>long unsigned int *vs_count</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*vs_dispatch)(struct svc_rqst *, __be32 *)</code> ➡️ <code>int (*vs_dispatch)(struct svc_rqst *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

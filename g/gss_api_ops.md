# Struct: <code>gss_api_ops</code>

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
struct gss_api_ops {
    int (*gss_import_sec_context)(const void *, size_t, struct gss_ctx *, time64_t *, gfp_t);
    u32 (*gss_get_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_verify_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_wrap)(struct gss_ctx *, int, struct xdr_buf *, struct page **);
    u32 (*gss_unwrap)(struct gss_ctx *, int, int, struct xdr_buf *);
    void (*gss_delete_sec_context)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct gss_api_ops {
    int (*gss_import_sec_context)(const void *, size_t, struct gss_ctx *, time64_t *, gfp_t);
    u32 (*gss_get_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_verify_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_wrap)(struct gss_ctx *, int, struct xdr_buf *, struct page **);
    u32 (*gss_unwrap)(struct gss_ctx *, int, int, struct xdr_buf *);
    void (*gss_delete_sec_context)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct gss_api_ops {
    int (*gss_import_sec_context)(const void *, size_t, struct gss_ctx *, time64_t *, gfp_t);
    u32 (*gss_get_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_verify_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_wrap)(struct gss_ctx *, int, struct xdr_buf *, struct page **);
    u32 (*gss_unwrap)(struct gss_ctx *, int, int, struct xdr_buf *);
    void (*gss_delete_sec_context)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct gss_api_ops {
    int (*gss_import_sec_context)(const void *, size_t, struct gss_ctx *, time64_t *, gfp_t);
    u32 (*gss_get_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_verify_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_wrap)(struct gss_ctx *, int, struct xdr_buf *, struct page **);
    u32 (*gss_unwrap)(struct gss_ctx *, int, int, struct xdr_buf *);
    void (*gss_delete_sec_context)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct gss_api_ops {
    int (*gss_import_sec_context)(const void *, size_t, struct gss_ctx *, time64_t *, gfp_t);
    u32 (*gss_get_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_verify_mic)(struct gss_ctx *, struct xdr_buf *, struct xdr_netobj *);
    u32 (*gss_wrap)(struct gss_ctx *, int, struct xdr_buf *, struct page **);
    u32 (*gss_unwrap)(struct gss_ctx *, int, int, struct xdr_buf *);
    void (*gss_delete_sec_context)(void *);
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

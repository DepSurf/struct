# Struct: <code>gnttab_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct gnttab_ops {
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct gnttab_ops {
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct gnttab_ops {
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct gnttab_ops {
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    long unsigned int (*read_frame)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t);
    long unsigned int (*read_frame)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t);
    long unsigned int (*read_frame)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t);
    long unsigned int (*read_frame)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t);
    long unsigned int (*read_frame)(grant_ref_t);
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
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct gnttab_ops {
    unsigned int version;
    unsigned int grefs_per_grant_frame;
    int (*map_frames)(xen_pfn_t *, unsigned int);
    void (*unmap_frames)();
    void (*update_entry)(grant_ref_t, domid_t, long unsigned int, unsigned int);
    int (*end_foreign_access_ref)(grant_ref_t, int);
    long unsigned int (*end_foreign_transfer_ref)(grant_ref_t);
    int (*query_foreign_access)(grant_ref_t);
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int version</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int grefs_per_grant_frame</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int (*read_frame)(grant_ref_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_foreign_access)(grant_ref_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int (*end_foreign_transfer_ref)(grant_ref_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*end_foreign_access_ref)(grant_ref_t, int)</code> ➡️ <code>int (*end_foreign_access_ref)(grant_ref_t)</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

# Struct: <code>ipv6_rpl_sr_hdr</code>

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
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ipv6_rpl_sr_hdr {
    __u8 nexthdr;
    __u8 hdrlen;
    __u8 type;
    __u8 segments_left;
    __u32 cmpre;
    __u32 cmpri;
    __u32 reserved;
    __u32 pad;
    __u32 reserved1;
    union (anon) segments;
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

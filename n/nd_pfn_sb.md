# Struct: <code>nd_pfn_sb</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    u8 padding[4012];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    u8 padding[4000];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
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
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
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
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
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
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nd_pfn_sb {
    u8 signature[16];
    u8 uuid[16];
    u8 parent_uuid[16];
    __le32 flags;
    __le16 version_major;
    __le16 version_minor;
    __le64 dataoff;
    __le64 npfns;
    __le32 mode;
    __le32 start_pad;
    __le32 end_trunc;
    __le32 align;
    __le32 page_size;
    __le16 page_struct_size;
    u8 padding[3994];
    __le64 checksum;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__le32 start_pad</code>
</li>
<li>
<b>Field added. </b>
<code>__le32 end_trunc</code>
</li>
<li>
<b>Field added. </b>
<code>__le32 align</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 padding[4012]</code> ➡️ <code>u8 padding[4000]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__le32 page_size</code>
</li>
<li>
<b>Field added. </b>
<code>__le16 page_struct_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 padding[4000]</code> ➡️ <code>u8 padding[3994]</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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

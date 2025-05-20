# Struct: <code>nd_namespace_label</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    __le32 unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    __le32 unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    __le32 unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nd_namespace_label {
    struct nvdimm_cxl_label cxl;
    struct nvdimm_efi_label efi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nd_namespace_label {
    struct nvdimm_cxl_label cxl;
    struct nvdimm_efi_label efi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nd_namespace_label {
    struct nvdimm_cxl_label cxl;
    struct nvdimm_efi_label efi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nd_namespace_label {
    struct nvdimm_cxl_label cxl;
    struct nvdimm_efi_label efi;
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
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
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
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
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
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
    __le64 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nd_namespace_label {
    u8 uuid[16];
    u8 name[64];
    __le32 flags;
    __le16 nlabel;
    __le16 position;
    __le64 isetcookie;
    __le64 lbasize;
    __le64 dpa;
    __le64 rawsize;
    __le32 slot;
    u8 align;
    u8 reserved[3];
    guid_t type_guid;
    guid_t abstraction_guid;
    u8 reserved2[88];
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 align</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved[3]</code>
</li>
<li>
<b>Field added. </b>
<code>guid_t type_guid</code>
</li>
<li>
<b>Field added. </b>
<code>guid_t abstraction_guid</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved2[88]</code>
</li>
<li>
<b>Field added. </b>
<code>__le64 checksum</code>
</li>
<li>
<b>Field removed. </b>
<code>__le32 unused</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct nvdimm_cxl_label cxl</code>
</li>
<li>
<b>Field added. </b>
<code>struct nvdimm_efi_label efi</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 uuid[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 name[64]</code>
</li>
<li>
<b>Field removed. </b>
<code>__le32 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>__le16 nlabel</code>
</li>
<li>
<b>Field removed. </b>
<code>__le16 position</code>
</li>
<li>
<b>Field removed. </b>
<code>__le64 isetcookie</code>
</li>
<li>
<b>Field removed. </b>
<code>__le64 lbasize</code>
</li>
<li>
<b>Field removed. </b>
<code>__le64 dpa</code>
</li>
<li>
<b>Field removed. </b>
<code>__le64 rawsize</code>
</li>
<li>
<b>Field removed. </b>
<code>__le32 slot</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 align</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>guid_t type_guid</code>
</li>
<li>
<b>Field removed. </b>
<code>guid_t abstraction_guid</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved2[88]</code>
</li>
<li>
<b>Field removed. </b>
<code>__le64 checksum</code>
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

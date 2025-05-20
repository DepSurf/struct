# Struct: <code>nvdimm_efi_label</code>

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
struct nvdimm_efi_label {
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
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nvdimm_efi_label {
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
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nvdimm_efi_label {
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
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nvdimm_efi_label {
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

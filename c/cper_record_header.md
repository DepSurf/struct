# Struct: <code>cper_record_header</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    uuid_le platform_id;
    uuid_le partition_id;
    uuid_le creator_id;
    uuid_le notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    uuid_le platform_id;
    uuid_le partition_id;
    uuid_le creator_id;
    uuid_le notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    uuid_le platform_id;
    uuid_le partition_id;
    uuid_le creator_id;
    uuid_le notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    uuid_le platform_id;
    uuid_le partition_id;
    uuid_le creator_id;
    uuid_le notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    __u16 revision;
    __u32 signature_end;
    __u16 section_count;
    __u32 error_severity;
    __u32 validation_bits;
    __u32 record_length;
    __u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    __u64 record_id;
    __u32 flags;
    __u64 persistence_information;
    __u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
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
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cper_record_header {
    char signature[4];
    u16 revision;
    u32 signature_end;
    u16 section_count;
    u32 error_severity;
    u32 validation_bits;
    u32 record_length;
    u64 timestamp;
    guid_t platform_id;
    guid_t partition_id;
    guid_t creator_id;
    guid_t notification_type;
    u64 record_id;
    u32 flags;
    u64 persistence_information;
    u8 reserved[12];
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
<b>Field type changed. </b>
<code>uuid_le platform_id</code> ➡️ <code>guid_t platform_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>uuid_le partition_id</code> ➡️ <code>guid_t partition_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>uuid_le creator_id</code> ➡️ <code>guid_t creator_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>uuid_le notification_type</code> ➡️ <code>guid_t notification_type</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__u16 revision</code> ➡️ <code>u16 revision</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 signature_end</code> ➡️ <code>u32 signature_end</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 section_count</code> ➡️ <code>u16 section_count</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 error_severity</code> ➡️ <code>u32 error_severity</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 validation_bits</code> ➡️ <code>u32 validation_bits</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 record_length</code> ➡️ <code>u32 record_length</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 timestamp</code> ➡️ <code>u64 timestamp</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 record_id</code> ➡️ <code>u64 record_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 flags</code> ➡️ <code>u32 flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 persistence_information</code> ➡️ <code>u64 persistence_information</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 reserved[12]</code> ➡️ <code>u8 reserved[12]</code>
</li>
</ul>
</details>
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
</ul>
<b>Flavor</b>
<ul>
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

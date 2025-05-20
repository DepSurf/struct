# Struct: <code>bpf_map_info</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
    __u64 map_extra;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
    __u64 map_extra;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
    __u64 map_extra;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u32 btf_vmlinux_value_type_id;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
    __u64 map_extra;
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
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
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
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_map_info {
    __u32 type;
    __u32 id;
    __u32 key_size;
    __u32 value_size;
    __u32 max_entries;
    __u32 map_flags;
    char name[16];
    __u32 ifindex;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 btf_id;
    __u32 btf_key_type_id;
    __u32 btf_value_type_id;
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>char name[16]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 ifindex</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 netns_dev</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 netns_ino</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 btf_key_type_id</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 btf_value_type_id</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 btf_vmlinux_value_type_id</code>
</li>
</ul>
</details>
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
<code>__u64 map_extra</code>
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
No changes between <code>amd64</code> and <code>armhf</code> ✅
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

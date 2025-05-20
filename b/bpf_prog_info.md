# Struct: <code>bpf_prog_info</code>

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
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
    __u64 recursion_misses;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
    __u64 recursion_misses;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
    __u64 recursion_misses;
    __u32 verified_insns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
    __u64 recursion_misses;
    __u32 verified_insns;
    __u32 attach_btf_obj_id;
    __u32 attach_btf_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
    __u64 recursion_misses;
    __u32 verified_insns;
    __u32 attach_btf_obj_id;
    __u32 attach_btf_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
    __u64 recursion_misses;
    __u32 verified_insns;
    __u32 attach_btf_obj_id;
    __u32 attach_btf_id;
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
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
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
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_prog_info {
    __u32 type;
    __u32 id;
    __u8 tag[8];
    __u32 jited_prog_len;
    __u32 xlated_prog_len;
    __u64 jited_prog_insns;
    __u64 xlated_prog_insns;
    __u64 load_time;
    __u32 created_by_uid;
    __u32 nr_map_ids;
    __u64 map_ids;
    char name[16];
    __u32 ifindex;
    __u32 gpl_compatible;
    __u64 netns_dev;
    __u64 netns_ino;
    __u32 nr_jited_ksyms;
    __u32 nr_jited_func_lens;
    __u64 jited_ksyms;
    __u64 jited_func_lens;
    __u32 btf_id;
    __u32 func_info_rec_size;
    __u64 func_info;
    __u32 nr_func_info;
    __u32 nr_line_info;
    __u64 line_info;
    __u64 jited_line_info;
    __u32 nr_jited_line_info;
    __u32 line_info_rec_size;
    __u32 jited_line_info_rec_size;
    __u32 nr_prog_tags;
    __u64 prog_tags;
    __u64 run_time_ns;
    __u64 run_cnt;
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
<code>__u64 load_time</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 created_by_uid</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 nr_map_ids</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 map_ids</code>
</li>
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
<code>__u32 gpl_compatible</code>
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
<code>__u32 nr_jited_ksyms</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 nr_jited_func_lens</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 jited_ksyms</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 jited_func_lens</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 func_info_rec_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 func_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 nr_func_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 nr_line_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 line_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 jited_line_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 nr_jited_line_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 line_info_rec_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 jited_line_info_rec_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 nr_prog_tags</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 prog_tags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 run_time_ns</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 run_cnt</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 recursion_misses</code>
</li>
</ul>
</details>
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
<code>__u32 verified_insns</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 attach_btf_obj_id</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 attach_btf_id</code>
</li>
</ul>
</details>
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

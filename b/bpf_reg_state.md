# Struct: <code>bpf_reg_state</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s64 imm;
    u16 off;
    u16 range;
    struct bpf_map *map_ptr;
    u32 id;
    s64 min_value;
    u64 max_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s64 imm;
    u16 off;
    u16 range;
    struct bpf_map *map_ptr;
    u32 id;
    s64 min_value;
    u64 max_value;
    u32 min_align;
    u32 aux_off;
    u32 aux_off_align;
    bool value_from_signed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    s32 off;
    u32 id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    enum bpf_reg_liveness live;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    s32 off;
    u32 id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    u32 frameno;
    enum bpf_reg_liveness live;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    enum bpf_reg_liveness live;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    u32 btf_id;
    u32 mem_size;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    struct (anon) raw;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    struct (anon) raw;
    u32 subprogno;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    u32 map_uid;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    struct (anon) raw;
    u32 subprogno;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    u32 map_uid;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    struct (anon) dynptr;
    struct (anon) raw;
    u32 subprogno;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    u32 map_uid;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    struct (anon) dynptr;
    struct (anon) raw;
    u32 subprogno;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    u32 map_uid;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    u32 dynptr_id;
    struct (anon) dynptr;
    struct (anon) iter;
    struct (anon) raw;
    u32 subprogno;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    u32 id;
    u32 ref_obj_id;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    s32 off;
    int range;
    struct bpf_map *map_ptr;
    u32 map_uid;
    struct btf *btf;
    u32 btf_id;
    u32 mem_size;
    u32 dynptr_id;
    struct (anon) dynptr;
    struct (anon) iter;
    struct (anon) raw;
    u32 subprogno;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    s32 s32_min_value;
    s32 s32_max_value;
    u32 u32_min_value;
    u32 u32_max_value;
    u32 id;
    u32 ref_obj_id;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
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
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
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
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_reg_state {
    enum bpf_reg_type type;
    u16 range;
    struct bpf_map *map_ptr;
    long unsigned int raw;
    s32 off;
    u32 id;
    u32 ref_obj_id;
    struct tnum var_off;
    s64 smin_value;
    s64 smax_value;
    u64 umin_value;
    u64 umax_value;
    struct bpf_reg_state *parent;
    u32 frameno;
    s32 subreg_def;
    enum bpf_reg_liveness live;
    bool precise;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 min_align</code>
</li>
<li>
<b>Field added. </b>
<code>u32 aux_off</code>
</li>
<li>
<b>Field added. </b>
<code>u32 aux_off_align</code>
</li>
<li>
<b>Field added. </b>
<code>bool value_from_signed</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tnum var_off</code>
</li>
<li>
<b>Field added. </b>
<code>s64 smin_value</code>
</li>
<li>
<b>Field added. </b>
<code>s64 smax_value</code>
</li>
<li>
<b>Field added. </b>
<code>u64 umin_value</code>
</li>
<li>
<b>Field added. </b>
<code>u64 umax_value</code>
</li>
<li>
<b>Field added. </b>
<code>enum bpf_reg_liveness live</code>
</li>
<li>
<b>Field removed. </b>
<code>s64 imm</code>
</li>
<li>
<b>Field removed. </b>
<code>s64 min_value</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 max_value</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 min_align</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 aux_off</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 aux_off_align</code>
</li>
<li>
<b>Field removed. </b>
<code>bool value_from_signed</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 off</code> ➡️ <code>s32 off</code>
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
<code>u32 frameno</code>
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
<code>long unsigned int raw</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_reg_state *parent</code>
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
<code>u32 ref_obj_id</code>
</li>
<li>
<b>Field added. </b>
<code>s32 subreg_def</code>
</li>
<li>
<b>Field added. </b>
<code>bool precise</code>
</li>
</ul>
</details>
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
<code>u32 btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 mem_size</code>
</li>
<li>
<b>Field added. </b>
<code>s32 s32_min_value</code>
</li>
<li>
<b>Field added. </b>
<code>s32 s32_max_value</code>
</li>
<li>
<b>Field added. </b>
<code>u32 u32_min_value</code>
</li>
<li>
<b>Field added. </b>
<code>u32 u32_max_value</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct btf *btf</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 range</code> ➡️ <code>int range</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int raw</code> ➡️ <code>struct (anon) raw</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 subprogno</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 map_uid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) dynptr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 dynptr_id</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) iter</code>
</li>
</ul>
</details>
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

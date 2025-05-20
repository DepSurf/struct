# Struct: <code>compat_fs_quota_stat</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct compat_fs_quota_stat {
    __s8 qs_version;
    __u16 qs_flags;
    __s8 qs_pad;
    struct compat_fs_qfilestat qs_uquota;
    struct compat_fs_qfilestat qs_gquota;
    compat_uint_t qs_incoredqs;
    compat_int_t qs_btimelimit;
    compat_int_t qs_itimelimit;
    compat_int_t qs_rtbtimelimit;
    __u16 qs_bwarnlimit;
    __u16 qs_iwarnlimit;
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

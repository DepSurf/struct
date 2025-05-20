# Struct: <code>compat_timex</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct compat_timeval time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct compat_timeval time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct compat_timeval time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct compat_timeval time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct compat_timeval time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct compat_timeval time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_timex {
    compat_uint_t modes;
    compat_long_t offset;
    compat_long_t freq;
    compat_long_t maxerror;
    compat_long_t esterror;
    compat_int_t status;
    compat_long_t constant;
    compat_long_t precision;
    compat_long_t tolerance;
    struct old_timeval32 time;
    compat_long_t tick;
    compat_long_t ppsfreq;
    compat_long_t jitter;
    compat_int_t shift;
    compat_long_t stabil;
    compat_long_t jitcnt;
    compat_long_t calcnt;
    compat_long_t errcnt;
    compat_long_t stbcnt;
    compat_int_t tai;
};
```
</details>
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
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct compat_timeval time</code> ➡️ <code>struct old_timeval32 time</code>
</li>
</ul>
</details>
</li>
</ul>

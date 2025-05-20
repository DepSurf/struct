# Struct: <code>devkmsg_user</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    enum log_flags prev;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    enum log_flags prev;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
    struct printk_info info;
    char text_buf[8192];
    struct printk_record record;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct devkmsg_user {
    atomic64_t seq;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
    struct printk_info info;
    char text_buf[8192];
    struct printk_record record;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct devkmsg_user {
    atomic64_t seq;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
    struct printk_info info;
    char text_buf[8192];
    struct printk_record record;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devkmsg_user {
    atomic64_t seq;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
    struct printk_info info;
    char text_buf[8192];
    struct printk_record record;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devkmsg_user {
    atomic64_t seq;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
    struct printk_info info;
    char text_buf[8192];
    struct printk_record record;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devkmsg_user {
    atomic64_t seq;
    struct ratelimit_state rs;
    struct mutex lock;
    struct printk_buffers pbufs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devkmsg_user {
    atomic64_t seq;
    struct ratelimit_state rs;
    struct mutex lock;
    struct printk_buffers pbufs;
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
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
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
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devkmsg_user {
    u64 seq;
    u32 idx;
    struct ratelimit_state rs;
    struct mutex lock;
    char buf[8192];
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
<code>struct ratelimit_state rs</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>enum log_flags prev</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct printk_info info</code>
</li>
<li>
<b>Field added. </b>
<code>char text_buf[8192]</code>
</li>
<li>
<b>Field added. </b>
<code>struct printk_record record</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 idx</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 seq</code> ➡️ <code>atomic64_t seq</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct printk_buffers pbufs</code>
</li>
<li>
<b>Field removed. </b>
<code>char buf[8192]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct printk_info info</code>
</li>
<li>
<b>Field removed. </b>
<code>char text_buf[8192]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct printk_record record</code>
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

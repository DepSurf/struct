# Struct: <code>n_tty_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    int minimum_to_wake;
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    size_t lookahead_count;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    size_t lookahead_count;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    unsigned int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    u8 read_buf[4096];
    long unsigned int read_flags[64];
    u8 echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    size_t lookahead_count;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
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
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[8];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[128];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
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
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct n_tty_data {
    size_t read_head;
    size_t commit_head;
    size_t canon_head;
    size_t echo_head;
    size_t echo_commit;
    size_t echo_mark;
    long unsigned int char_map[4];
    long unsigned int overrun_time;
    int num_overrun;
    bool no_room;
    unsigned char lnext;
    unsigned char erasing;
    unsigned char raw;
    unsigned char real_raw;
    unsigned char icanon;
    unsigned char push;
    char read_buf[4096];
    long unsigned int read_flags[64];
    unsigned char echo_buf[4096];
    size_t read_tail;
    size_t line_start;
    unsigned int column;
    unsigned int canon_column;
    size_t echo_tail;
    struct mutex atomic_read_lock;
    struct mutex output_lock;
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
<b>Field removed. </b>
<code>int minimum_to_wake</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t lookahead_count</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int num_overrun</code> ➡️ <code>unsigned int num_overrun</code>
</li>
<li>
<b>Field type changed. </b>
<code>char read_buf[4096]</code> ➡️ <code>u8 read_buf[4096]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char echo_buf[4096]</code> ➡️ <code>u8 echo_buf[4096]</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int char_map[4]</code> ➡️ <code>long unsigned int char_map[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int read_flags[64]</code> ➡️ <code>long unsigned int read_flags[128]</code>
</li>
</ul>
</details>
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

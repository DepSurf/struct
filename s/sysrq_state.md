# Struct: <code>sysrq_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    unsigned int shift;
    unsigned int shift_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
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
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[24];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[24];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
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
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sysrq_state {
    struct input_handle handle;
    struct work_struct reinject_work;
    long unsigned int key_down[12];
    unsigned int alt;
    unsigned int alt_use;
    bool active;
    bool need_reinject;
    bool reinjecting;
    bool reset_canceled;
    bool reset_requested;
    long unsigned int reset_keybit[12];
    int reset_seq_len;
    int reset_seq_cnt;
    int reset_seq_version;
    struct timer_list keyreset_timer;
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int shift</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int shift_use</code>
</li>
</ul>
</details>
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
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int key_down[12]</code> ➡️ <code>long unsigned int key_down[24]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int reset_keybit[12]</code> ➡️ <code>long unsigned int reset_keybit[24]</code>
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

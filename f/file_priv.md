# Struct: <code>file_priv</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    atomic_t data_pending;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct work;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    atomic_t data_pending;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct work;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    atomic_t data_pending;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct work;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    atomic_t data_pending;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct work;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    atomic_t data_pending;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct work;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    size_t data_pending;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct work;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    size_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    size_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
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
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
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
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct file_priv {
    struct tpm_chip *chip;
    struct tpm_space *space;
    struct mutex buffer_mutex;
    struct timer_list user_read_timer;
    struct work_struct timeout_work;
    struct work_struct async_work;
    wait_queue_head_t async_wait;
    ssize_t response_length;
    bool response_read;
    bool command_enqueued;
    u8 data_buffer[4096];
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t data_pending</code> ➡️ <code>size_t data_pending</code>
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
<code>struct tpm_space *space</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct timeout_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct async_work</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t async_wait</code>
</li>
<li>
<b>Field added. </b>
<code>size_t response_length</code>
</li>
<li>
<b>Field added. </b>
<code>bool response_read</code>
</li>
<li>
<b>Field added. </b>
<code>bool command_enqueued</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t data_pending</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct work</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>size_t response_length</code> ➡️ <code>ssize_t response_length</code>
</li>
</ul>
</details>
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

# Struct: <code>posix_clock_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec *);
    int (*clock_getres)(struct posix_clock *, struct timespec *);
    int (*clock_settime)(struct posix_clock *, const struct timespec *);
    int (*timer_create)(struct posix_clock *, struct k_itimer *);
    int (*timer_delete)(struct posix_clock *, struct k_itimer *);
    void (*timer_gettime)(struct posix_clock *, struct k_itimer *, struct itimerspec *);
    int (*timer_settime)(struct posix_clock *, struct k_itimer *, int, struct itimerspec *, struct itimerspec *);
    int (*fasync)(struct posix_clock *, int, struct file *, int);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*mmap)(struct posix_clock *, struct vm_area_struct *);
    int (*open)(struct posix_clock *, fmode_t);
    uint (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec *);
    int (*clock_getres)(struct posix_clock *, struct timespec *);
    int (*clock_settime)(struct posix_clock *, const struct timespec *);
    int (*timer_create)(struct posix_clock *, struct k_itimer *);
    int (*timer_delete)(struct posix_clock *, struct k_itimer *);
    void (*timer_gettime)(struct posix_clock *, struct k_itimer *, struct itimerspec *);
    int (*timer_settime)(struct posix_clock *, struct k_itimer *, int, struct itimerspec *, struct itimerspec *);
    int (*fasync)(struct posix_clock *, int, struct file *, int);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*mmap)(struct posix_clock *, struct vm_area_struct *);
    int (*open)(struct posix_clock *, fmode_t);
    uint (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec *);
    int (*clock_getres)(struct posix_clock *, struct timespec *);
    int (*clock_settime)(struct posix_clock *, const struct timespec *);
    int (*timer_create)(struct posix_clock *, struct k_itimer *);
    int (*timer_delete)(struct posix_clock *, struct k_itimer *);
    void (*timer_gettime)(struct posix_clock *, struct k_itimer *, struct itimerspec *);
    int (*timer_settime)(struct posix_clock *, struct k_itimer *, int, struct itimerspec *, struct itimerspec *);
    int (*fasync)(struct posix_clock *, int, struct file *, int);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*mmap)(struct posix_clock *, struct vm_area_struct *);
    int (*open)(struct posix_clock *, fmode_t);
    uint (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec *);
    int (*clock_getres)(struct posix_clock *, struct timespec *);
    int (*clock_settime)(struct posix_clock *, const struct timespec *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    uint (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec *);
    int (*clock_getres)(struct posix_clock *, struct timespec *);
    int (*clock_settime)(struct posix_clock *, const struct timespec *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    uint (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock_context *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock_context *, fmode_t);
    __poll_t (*poll)(struct posix_clock_context *, struct file *, poll_table *);
    int (*release)(struct posix_clock_context *);
    ssize_t (*read)(struct posix_clock_context *, uint, char *, size_t);
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
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
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
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct posix_clock_operations {
    struct module *owner;
    int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *);
    int (*clock_gettime)(struct posix_clock *, struct timespec64 *);
    int (*clock_getres)(struct posix_clock *, struct timespec64 *);
    int (*clock_settime)(struct posix_clock *, const struct timespec64 *);
    long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int);
    int (*open)(struct posix_clock *, fmode_t);
    __poll_t (*poll)(struct posix_clock *, struct file *, poll_table *);
    int (*release)(struct posix_clock *);
    ssize_t (*read)(struct posix_clock *, uint, char *, size_t);
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*timer_create)(struct posix_clock *, struct k_itimer *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*timer_delete)(struct posix_clock *, struct k_itimer *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*timer_gettime)(struct posix_clock *, struct k_itimer *, struct itimerspec *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*timer_settime)(struct posix_clock *, struct k_itimer *, int, struct itimerspec *, struct itimerspec *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*fasync)(struct posix_clock *, int, struct file *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mmap)(struct posix_clock *, struct vm_area_struct *)</code>
</li>
</ul>
</details>
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
<code>int (*clock_gettime)(struct posix_clock *, struct timespec *)</code> ➡️ <code>int (*clock_gettime)(struct posix_clock *, struct timespec64 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*clock_getres)(struct posix_clock *, struct timespec *)</code> ➡️ <code>int (*clock_getres)(struct posix_clock *, struct timespec64 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*clock_settime)(struct posix_clock *, const struct timespec *)</code> ➡️ <code>int (*clock_settime)(struct posix_clock *, const struct timespec64 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>uint (*poll)(struct posix_clock *, struct file *, poll_table *)</code> ➡️ <code>__poll_t (*poll)(struct posix_clock *, struct file *, poll_table *)</code>
</li>
</ul>
</details>
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
<code>int (*clock_adjtime)(struct posix_clock *, struct timex *)</code> ➡️ <code>int (*clock_adjtime)(struct posix_clock *, struct __kernel_timex *)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int (*ioctl)(struct posix_clock *, unsigned int, long unsigned int)</code> ➡️ <code>long int (*ioctl)(struct posix_clock_context *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*open)(struct posix_clock *, fmode_t)</code> ➡️ <code>int (*open)(struct posix_clock_context *, fmode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>__poll_t (*poll)(struct posix_clock *, struct file *, poll_table *)</code> ➡️ <code>__poll_t (*poll)(struct posix_clock_context *, struct file *, poll_table *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*release)(struct posix_clock *)</code> ➡️ <code>int (*release)(struct posix_clock_context *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*read)(struct posix_clock *, uint, char *, size_t)</code> ➡️ <code>ssize_t (*read)(struct posix_clock_context *, uint, char *, size_t)</code>
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

# Struct: <code>sdio_func</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 tmpbuf[4];
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 tmpbuf[4];
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 tmpbuf[4];
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
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
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
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
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sdio_func {
    struct mmc_card *card;
    struct device dev;
    sdio_irq_handler_t *irq_handler;
    unsigned int num;
    unsigned char class;
    short unsigned int vendor;
    short unsigned int device;
    unsigned int max_blksize;
    unsigned int cur_blksize;
    unsigned int enable_timeout;
    unsigned int state;
    u8 *tmpbuf;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
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
<b>Field type changed. </b>
<code>u8 tmpbuf[4]</code> ➡️ <code>u8 *tmpbuf</code>
</li>
</ul>
</details>
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
<code>u8 major_rev</code>
</li>
<li>
<b>Field added. </b>
<code>u8 minor_rev</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

# Struct: <code>spi_transfer</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    u32 speed_hz;
    u16 word_delay;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    bool timestamped;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u16 delay_usecs;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    bool timestamped;
    struct list_head transfer_list;
    u16 error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int dummy_data;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    bool timestamped;
    struct list_head transfer_list;
    u16 error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int dummy_data;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    bool timestamped;
    struct list_head transfer_list;
    u16 error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int dummy_data;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    bool timestamped;
    struct list_head transfer_list;
    u16 error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int dummy_data;
    unsigned int cs_off;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    bool timestamped;
    struct list_head transfer_list;
    u16 error;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    u16 error;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int dummy_data;
    unsigned int cs_off;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    unsigned int timestamped;
    u8 bits_per_word;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    u16 error;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int dummy_data;
    unsigned int cs_off;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    unsigned int timestamped;
    u8 bits_per_word;
    struct spi_delay delay;
    struct spi_delay cs_change_delay;
    struct spi_delay word_delay;
    u32 speed_hz;
    u32 effective_speed_hz;
    unsigned int ptp_sts_word_pre;
    unsigned int ptp_sts_word_post;
    struct ptp_system_timestamp *ptp_sts;
    struct list_head transfer_list;
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
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
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
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct spi_transfer {
    const void *tx_buf;
    void *rx_buf;
    unsigned int len;
    dma_addr_t tx_dma;
    dma_addr_t rx_dma;
    struct sg_table tx_sg;
    struct sg_table rx_sg;
    unsigned int cs_change;
    unsigned int tx_nbits;
    unsigned int rx_nbits;
    u8 bits_per_word;
    u8 word_delay_usecs;
    u16 delay_usecs;
    u16 cs_change_delay;
    u8 cs_change_delay_unit;
    u32 speed_hz;
    u16 word_delay;
    u32 effective_speed_hz;
    struct list_head transfer_list;
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 word_delay</code>
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
<code>u8 word_delay_usecs</code>
</li>
<li>
<b>Field added. </b>
<code>u16 cs_change_delay</code>
</li>
<li>
<b>Field added. </b>
<code>u8 cs_change_delay_unit</code>
</li>
<li>
<b>Field added. </b>
<code>u32 effective_speed_hz</code>
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
<code>struct spi_delay delay</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ptp_sts_word_pre</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ptp_sts_word_post</code>
</li>
<li>
<b>Field added. </b>
<code>struct ptp_system_timestamp *ptp_sts</code>
</li>
<li>
<b>Field added. </b>
<code>bool timestamped</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 word_delay_usecs</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 cs_change_delay_unit</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 cs_change_delay</code> ➡️ <code>struct spi_delay cs_change_delay</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 word_delay</code> ➡️ <code>struct spi_delay word_delay</code>
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
<code>u16 error</code>
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
<code>unsigned int dummy_data</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 delay_usecs</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int cs_off</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>bool timestamped</code> ➡️ <code>unsigned int timestamped</code>
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

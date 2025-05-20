# Struct: <code>spi_statistics</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct spi_statistics {
    struct u64_stats_sync syncp;
    u64_stats_t messages;
    u64_stats_t transfers;
    u64_stats_t errors;
    u64_stats_t timedout;
    u64_stats_t spi_sync;
    u64_stats_t spi_sync_immediate;
    u64_stats_t spi_async;
    u64_stats_t bytes;
    u64_stats_t bytes_rx;
    u64_stats_t bytes_tx;
    u64_stats_t transfer_bytes_histo[17];
    u64_stats_t transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct spi_statistics {
    struct u64_stats_sync syncp;
    u64_stats_t messages;
    u64_stats_t transfers;
    u64_stats_t errors;
    u64_stats_t timedout;
    u64_stats_t spi_sync;
    u64_stats_t spi_sync_immediate;
    u64_stats_t spi_async;
    u64_stats_t bytes;
    u64_stats_t bytes_rx;
    u64_stats_t bytes_tx;
    u64_stats_t transfer_bytes_histo[17];
    u64_stats_t transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct spi_statistics {
    struct u64_stats_sync syncp;
    u64_stats_t messages;
    u64_stats_t transfers;
    u64_stats_t errors;
    u64_stats_t timedout;
    u64_stats_t spi_sync;
    u64_stats_t spi_sync_immediate;
    u64_stats_t spi_async;
    u64_stats_t bytes;
    u64_stats_t bytes_rx;
    u64_stats_t bytes_tx;
    u64_stats_t transfer_bytes_histo[17];
    u64_stats_t transfers_split_maxsize;
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
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
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
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct spi_statistics {
    spinlock_t lock;
    long unsigned int messages;
    long unsigned int transfers;
    long unsigned int errors;
    long unsigned int timedout;
    long unsigned int spi_sync;
    long unsigned int spi_sync_immediate;
    long unsigned int spi_async;
    long long unsigned int bytes;
    long long unsigned int bytes_rx;
    long long unsigned int bytes_tx;
    long unsigned int transfer_bytes_histo[17];
    long unsigned int transfers_split_maxsize;
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
<code>long unsigned int transfers_split_maxsize</code>
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
<code>struct u64_stats_sync syncp</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int messages</code> ➡️ <code>u64_stats_t messages</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int transfers</code> ➡️ <code>u64_stats_t transfers</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int errors</code> ➡️ <code>u64_stats_t errors</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int timedout</code> ➡️ <code>u64_stats_t timedout</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int spi_sync</code> ➡️ <code>u64_stats_t spi_sync</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int spi_sync_immediate</code> ➡️ <code>u64_stats_t spi_sync_immediate</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int spi_async</code> ➡️ <code>u64_stats_t spi_async</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long unsigned int bytes</code> ➡️ <code>u64_stats_t bytes</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long unsigned int bytes_rx</code> ➡️ <code>u64_stats_t bytes_rx</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long unsigned int bytes_tx</code> ➡️ <code>u64_stats_t bytes_tx</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int transfer_bytes_histo[17]</code> ➡️ <code>u64_stats_t transfer_bytes_histo[17]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int transfers_split_maxsize</code> ➡️ <code>u64_stats_t transfers_split_maxsize</code>
</li>
</ul>
</details>
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

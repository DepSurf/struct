# Struct: <code>throtl_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int nr_undestroyed_grps;
    struct work_struct dispatch_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    struct work_struct dispatch_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    struct work_struct dispatch_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[9];
    struct avg_latency_bucket avg_buckets[9];
    struct latency_bucket *latency_buckets;
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[9];
    struct avg_latency_bucket avg_buckets[9];
    struct latency_bucket *latency_buckets;
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
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
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
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
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct throtl_data {
    struct throtl_service_queue service_queue;
    struct request_queue *queue;
    unsigned int nr_queued[2];
    unsigned int throtl_slice;
    struct work_struct dispatch_work;
    unsigned int limit_index;
    bool limit_valid[2];
    long unsigned int low_upgrade_time;
    long unsigned int low_downgrade_time;
    unsigned int scale;
    struct latency_bucket tmp_buckets[18];
    struct avg_latency_bucket avg_buckets[18];
    struct latency_bucket * latency_buckets[2];
    long unsigned int last_calculate_time;
    long unsigned int filtered_latency;
    bool track_bio_latency;
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
<code>unsigned int nr_undestroyed_grps</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int throtl_slice</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int limit_index</code>
</li>
<li>
<b>Field added. </b>
<code>bool limit_valid[2]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int low_upgrade_time</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int low_downgrade_time</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int scale</code>
</li>
<li>
<b>Field added. </b>
<code>struct latency_bucket tmp_buckets[9]</code>
</li>
<li>
<b>Field added. </b>
<code>struct avg_latency_bucket avg_buckets[9]</code>
</li>
<li>
<b>Field added. </b>
<code>struct latency_bucket *latency_buckets</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int last_calculate_time</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int filtered_latency</code>
</li>
<li>
<b>Field added. </b>
<code>bool track_bio_latency</code>
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
<code>struct latency_bucket tmp_buckets[9]</code> ➡️ <code>struct latency_bucket tmp_buckets[18]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct avg_latency_bucket avg_buckets[9]</code> ➡️ <code>struct avg_latency_bucket avg_buckets[18]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct latency_bucket *latency_buckets</code> ➡️ <code>struct latency_bucket * latency_buckets[2]</code>
</li>
</ul>
</details>
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

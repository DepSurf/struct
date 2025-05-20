# Struct: <code>rq_wb</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    unsigned int wb_max;
    int scale_step;
    bool scaled_max;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct timer_list window_timer;
    s64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    unsigned int queue_depth;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct request_queue *queue;
    struct rq_wait rq_wait[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    unsigned int wb_max;
    int scale_step;
    bool scaled_max;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    s64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    unsigned int queue_depth;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct request_queue *queue;
    struct rq_wait rq_wait[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    unsigned int wb_max;
    int scale_step;
    bool scaled_max;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    s64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    unsigned int queue_depth;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct request_queue *queue;
    struct rq_wait rq_wait[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    unsigned int wb_max;
    int scale_step;
    bool scaled_max;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    unsigned int queue_depth;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct request_queue *queue;
    struct rq_wait rq_wait[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
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
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
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
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rq_wb {
    unsigned int wb_background;
    unsigned int wb_normal;
    short int enable_state;
    unsigned int unknown_cnt;
    u64 win_nsec;
    u64 cur_win_nsec;
    struct blk_stat_callback *cb;
    u64 sync_issue;
    void *sync_cookie;
    unsigned int wc;
    long unsigned int last_issue;
    long unsigned int last_comp;
    long unsigned int min_lat_nsec;
    struct rq_qos rqos;
    struct rq_wait rq_wait[3];
    struct rq_depth rq_depth;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct blk_stat_callback *cb</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list window_timer</code>
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
<code>s64 sync_issue</code> ➡️ <code>u64 sync_issue</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rq_wait rq_wait[2]</code> ➡️ <code>struct rq_wait rq_wait[3]</code>
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
<code>struct rq_qos rqos</code>
</li>
<li>
<b>Field added. </b>
<code>struct rq_depth rq_depth</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int wb_max</code>
</li>
<li>
<b>Field removed. </b>
<code>int scale_step</code>
</li>
<li>
<b>Field removed. </b>
<code>bool scaled_max</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int queue_depth</code>
</li>
<li>
<b>Field removed. </b>
<code>struct request_queue *queue</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int wc</code>
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

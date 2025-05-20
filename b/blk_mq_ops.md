# Struct: <code>blk_mq_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    map_queue_fn *map_queue;
    timeout_fn *timeout;
    poll_fn *poll;
    softirq_done_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    map_queue_fn *map_queue;
    timeout_fn *timeout;
    poll_fn *poll;
    softirq_done_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    reinit_request_fn *reinit_request;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    timeout_fn *timeout;
    poll_fn *poll;
    softirq_done_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    reinit_request_fn *reinit_request;
    map_queues_fn *map_queues;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    timeout_fn *timeout;
    poll_fn *poll;
    softirq_done_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    reinit_request_fn *reinit_request;
    void (*initialize_rq_fn)(struct request *);
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    softirq_done_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    softirq_done_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    bool (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *);
    enum blk_eh_timer_return (*timeout)(struct request *, bool);
    int (*poll)(struct blk_mq_hw_ctx *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*initialize_rq_fn)(struct request *);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    int (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    int (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *, int);
    void (*set_rq_budget_token)(struct request *, int);
    int (*get_rq_budget_token)(struct request *);
    enum blk_eh_timer_return (*timeout)(struct request *, bool);
    int (*poll)(struct blk_mq_hw_ctx *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*initialize_rq_fn)(struct request *);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    int (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    int (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *, int);
    void (*set_rq_budget_token)(struct request *, int);
    int (*get_rq_budget_token)(struct request *);
    enum blk_eh_timer_return (*timeout)(struct request *, bool);
    int (*poll)(struct blk_mq_hw_ctx *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*initialize_rq_fn)(struct request *);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    int (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    void (*queue_rqs)(struct request **);
    int (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *, int);
    void (*set_rq_budget_token)(struct request *, int);
    int (*get_rq_budget_token)(struct request *);
    enum blk_eh_timer_return (*timeout)(struct request *, bool);
    int (*poll)(struct blk_mq_hw_ctx *, struct io_comp_batch *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    int (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    void (*queue_rqs)(struct request **);
    int (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *, int);
    void (*set_rq_budget_token)(struct request *, int);
    int (*get_rq_budget_token)(struct request *);
    enum blk_eh_timer_return (*timeout)(struct request *);
    int (*poll)(struct blk_mq_hw_ctx *, struct io_comp_batch *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    void (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    void (*queue_rqs)(struct request **);
    int (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *, int);
    void (*set_rq_budget_token)(struct request *, int);
    int (*get_rq_budget_token)(struct request *);
    enum blk_eh_timer_return (*timeout)(struct request *);
    int (*poll)(struct blk_mq_hw_ctx *, struct io_comp_batch *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    void (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blk_mq_ops {
    blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *);
    void (*commit_rqs)(struct blk_mq_hw_ctx *);
    void (*queue_rqs)(struct request **);
    int (*get_budget)(struct request_queue *);
    void (*put_budget)(struct request_queue *, int);
    void (*set_rq_budget_token)(struct request *, int);
    int (*get_rq_budget_token)(struct request *);
    enum blk_eh_timer_return (*timeout)(struct request *);
    int (*poll)(struct blk_mq_hw_ctx *, struct io_comp_batch *);
    void (*complete)(struct request *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int);
    void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int);
    void (*cleanup_rq)(struct request *);
    bool (*busy)(struct request_queue *);
    void (*map_queues)(struct blk_mq_tag_set *);
    void (*show_rq)(struct seq_file *, struct request *);
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
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
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
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blk_mq_ops {
    queue_rq_fn *queue_rq;
    commit_rqs_fn *commit_rqs;
    get_budget_fn *get_budget;
    put_budget_fn *put_budget;
    timeout_fn *timeout;
    poll_fn *poll;
    complete_fn *complete;
    init_hctx_fn *init_hctx;
    exit_hctx_fn *exit_hctx;
    init_request_fn *init_request;
    exit_request_fn *exit_request;
    void (*initialize_rq_fn)(struct request *);
    cleanup_rq_fn *cleanup_rq;
    busy_fn *busy;
    map_queues_fn *map_queues;
    void (*show_rq)(struct seq_file *, struct request *);
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
<code>reinit_request_fn *reinit_request</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>map_queues_fn *map_queues</code>
</li>
<li>
<b>Field removed. </b>
<code>map_queue_fn *map_queue</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*initialize_rq_fn)(struct request *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*show_rq)(struct seq_file *, struct request *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>get_budget_fn *get_budget</code>
</li>
<li>
<b>Field added. </b>
<code>put_budget_fn *put_budget</code>
</li>
<li>
<b>Field removed. </b>
<code>reinit_request_fn *reinit_request</code>
</li>
</ul>
</details>
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
<code>commit_rqs_fn *commit_rqs</code>
</li>
<li>
<b>Field added. </b>
<code>busy_fn *busy</code>
</li>
<li>
<b>Field type changed. </b>
<code>softirq_done_fn *complete</code> ➡️ <code>complete_fn *complete</code>
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
<b>Field added. </b>
<code>cleanup_rq_fn *cleanup_rq</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>queue_rq_fn *queue_rq</code> ➡️ <code>blk_status_t (*queue_rq)(struct blk_mq_hw_ctx *, const struct blk_mq_queue_data *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>commit_rqs_fn *commit_rqs</code> ➡️ <code>void (*commit_rqs)(struct blk_mq_hw_ctx *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>get_budget_fn *get_budget</code> ➡️ <code>bool (*get_budget)(struct request_queue *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>put_budget_fn *put_budget</code> ➡️ <code>void (*put_budget)(struct request_queue *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>timeout_fn *timeout</code> ➡️ <code>enum blk_eh_timer_return (*timeout)(struct request *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>poll_fn *poll</code> ➡️ <code>int (*poll)(struct blk_mq_hw_ctx *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>complete_fn *complete</code> ➡️ <code>void (*complete)(struct request *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>init_hctx_fn *init_hctx</code> ➡️ <code>int (*init_hctx)(struct blk_mq_hw_ctx *, void *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>exit_hctx_fn *exit_hctx</code> ➡️ <code>void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>init_request_fn *init_request</code> ➡️ <code>int (*init_request)(struct blk_mq_tag_set *, struct request *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>exit_request_fn *exit_request</code> ➡️ <code>void (*exit_request)(struct blk_mq_tag_set *, struct request *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>cleanup_rq_fn *cleanup_rq</code> ➡️ <code>void (*cleanup_rq)(struct request *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>busy_fn *busy</code> ➡️ <code>bool (*busy)(struct request_queue *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>map_queues_fn *map_queues</code> ➡️ <code>int (*map_queues)(struct blk_mq_tag_set *)</code>
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
<code>void (*set_rq_budget_token)(struct request *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_rq_budget_token)(struct request *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*get_budget)(struct request_queue *)</code> ➡️ <code>int (*get_budget)(struct request_queue *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*put_budget)(struct request_queue *)</code> ➡️ <code>void (*put_budget)(struct request_queue *, int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*queue_rqs)(struct request **)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*initialize_rq_fn)(struct request *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*poll)(struct blk_mq_hw_ctx *)</code> ➡️ <code>int (*poll)(struct blk_mq_hw_ctx *, struct io_comp_batch *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>enum blk_eh_timer_return (*timeout)(struct request *, bool)</code> ➡️ <code>enum blk_eh_timer_return (*timeout)(struct request *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_queues)(struct blk_mq_tag_set *)</code> ➡️ <code>void (*map_queues)(struct blk_mq_tag_set *)</code>
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

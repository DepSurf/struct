# Struct: <code>elevator_mq_ops</code>

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
In <code>4.10</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *);
    void (*started_request)(struct request *);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *);
    void (*started_request)(struct request *);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *);
    void (*started_request)(struct request *);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*started_request)(struct request *);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(blk_opf_t, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(blk_opf_t, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, blk_insert_t);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(blk_opf_t, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, blk_insert_t);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
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
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
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
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct elevator_mq_ops {
    int (*init_sched)(struct request_queue *, struct elevator_type *);
    void (*exit_sched)(struct elevator_queue *);
    int (*init_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*exit_hctx)(struct blk_mq_hw_ctx *, unsigned int);
    void (*depth_updated)(struct blk_mq_hw_ctx *);
    bool (*allow_merge)(struct request_queue *, struct request *, struct bio *);
    bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int);
    int (*request_merge)(struct request_queue *, struct request **, struct bio *);
    void (*request_merged)(struct request_queue *, struct request *, enum elv_merge);
    void (*requests_merged)(struct request_queue *, struct request *, struct request *);
    void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *);
    void (*prepare_request)(struct request *, struct bio *);
    void (*finish_request)(struct request *);
    void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool);
    struct request * (*dispatch_request)(struct blk_mq_hw_ctx *);
    bool (*has_work)(struct blk_mq_hw_ctx *);
    void (*completed_request)(struct request *, u64);
    void (*requeue_request)(struct request *);
    struct request * (*former_request)(struct request_queue *, struct request *);
    struct request * (*next_request)(struct request_queue *, struct request *);
    void (*init_icq)(struct io_cq *);
    void (*exit_icq)(struct io_cq *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<b>Field type changed. </b>
<code>void (*completed_request)(struct request *)</code> ➡️ <code>void (*completed_request)(struct request *, u64)</code>
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
<code>void (*depth_updated)(struct blk_mq_hw_ctx *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*started_request)(struct request *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *)</code> ➡️ <code>bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int)</code>
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
<b>Field type changed. </b>
<code>void (*prepare_request)(struct request *, struct bio *)</code> ➡️ <code>void (*prepare_request)(struct request *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>bool (*bio_merge)(struct blk_mq_hw_ctx *, struct bio *, unsigned int)</code> ➡️ <code>bool (*bio_merge)(struct request_queue *, struct bio *, unsigned int)</code>
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
<b>Field type changed. </b>
<code>void (*limit_depth)(unsigned int, struct blk_mq_alloc_data *)</code> ➡️ <code>void (*limit_depth)(blk_opf_t, struct blk_mq_alloc_data *)</code>
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
<code>void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, bool)</code> ➡️ <code>void (*insert_requests)(struct blk_mq_hw_ctx *, struct list_head *, blk_insert_t)</code>
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

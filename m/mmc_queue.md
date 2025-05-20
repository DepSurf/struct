# Struct: <code>mmc_queue</code>

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
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct mmc_queue {
    struct mmc_card *card;
    struct mmc_ctx ctx;
    struct blk_mq_tag_set tag_set;
    struct mmc_blk_data *blkdata;
    struct request_queue *queue;
    spinlock_t lock;
    int in_flight[3];
    unsigned int cqe_busy;
    bool busy;
    bool use_cqe;
    bool recovery_needed;
    bool in_recovery;
    bool rw_wait;
    bool waiting;
    struct work_struct recovery_work;
    wait_queue_head_t wait;
    struct request *recovery_req;
    struct request *complete_req;
    struct mutex complete_lock;
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_queue {
    struct mmc_card *card;
    struct mmc_ctx ctx;
    struct blk_mq_tag_set tag_set;
    struct mmc_blk_data *blkdata;
    struct request_queue *queue;
    spinlock_t lock;
    int in_flight[3];
    unsigned int cqe_busy;
    bool busy;
    bool use_cqe;
    bool recovery_needed;
    bool in_recovery;
    bool rw_wait;
    bool waiting;
    struct work_struct recovery_work;
    wait_queue_head_t wait;
    struct request *recovery_req;
    struct request *complete_req;
    struct mutex complete_lock;
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_queue {
    struct mmc_card *card;
    struct mmc_ctx ctx;
    struct blk_mq_tag_set tag_set;
    struct mmc_blk_data *blkdata;
    struct request_queue *queue;
    spinlock_t lock;
    int in_flight[3];
    unsigned int cqe_busy;
    bool busy;
    bool use_cqe;
    bool recovery_needed;
    bool in_recovery;
    bool rw_wait;
    bool waiting;
    struct work_struct recovery_work;
    wait_queue_head_t wait;
    struct request *recovery_req;
    struct request *complete_req;
    struct mutex complete_lock;
    struct work_struct complete_work;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>

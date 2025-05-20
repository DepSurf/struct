# Struct: <code>throtl_grp</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[2];
    unsigned int iops[2];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[2];
    unsigned int iops[2];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[2];
    unsigned int iops[2];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    atomic_t io_split_cnt[2];
    atomic_t last_io_split_cnt[2];
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules_bps[2];
    bool has_rules_iops[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    uint64_t carryover_bytes[2];
    unsigned int carryover_ios[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules_bps[2];
    bool has_rules_iops[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    uint64_t carryover_bytes[2];
    unsigned int carryover_ios[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules_bps[2];
    bool has_rules_iops[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long long int carryover_bytes[2];
    int carryover_ios[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
    struct blkg_rwstat stat_bytes;
    struct blkg_rwstat stat_ios;
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
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
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
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct throtl_grp {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    struct throtl_data *td;
    struct throtl_service_queue service_queue;
    struct throtl_qnode qnode_on_self[2];
    struct throtl_qnode qnode_on_parent[2];
    long unsigned int disptime;
    unsigned int flags;
    bool has_rules[2];
    uint64_t bps[4];
    uint64_t bps_conf[4];
    unsigned int iops[4];
    unsigned int iops_conf[4];
    uint64_t bytes_disp[2];
    unsigned int io_disp[2];
    long unsigned int last_low_overflow_time[2];
    uint64_t last_bytes_disp[2];
    unsigned int last_io_disp[2];
    long unsigned int last_check_time;
    long unsigned int latency_target;
    long unsigned int latency_target_conf;
    long unsigned int slice_start[2];
    long unsigned int slice_end[2];
    long unsigned int last_finish_time;
    long unsigned int checked_last_finish_time;
    long unsigned int avg_idletime;
    long unsigned int idletime_threshold;
    long unsigned int idletime_threshold_conf;
    unsigned int bio_cnt;
    unsigned int bad_bio_cnt;
    long unsigned int bio_cnt_reset_time;
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
<b>Field added. </b>
<code>uint64_t bps_conf[4]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int iops_conf[4]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int last_low_overflow_time[2]</code>
</li>
<li>
<b>Field added. </b>
<code>uint64_t last_bytes_disp[2]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int last_io_disp[2]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int last_check_time</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int latency_target</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int latency_target_conf</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int last_finish_time</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int checked_last_finish_time</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int avg_idletime</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int idletime_threshold</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int idletime_threshold_conf</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int bio_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int bad_bio_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int bio_cnt_reset_time</code>
</li>
<li>
<b>Field type changed. </b>
<code>uint64_t bps[2]</code> ➡️ <code>uint64_t bps[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int iops[2]</code> ➡️ <code>unsigned int iops[4]</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct blkg_rwstat stat_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>struct blkg_rwstat stat_ios</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t io_split_cnt[2]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t last_io_split_cnt[2]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t io_split_cnt[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t last_io_split_cnt[2]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool has_rules_bps[2]</code>
</li>
<li>
<b>Field added. </b>
<code>bool has_rules_iops[2]</code>
</li>
<li>
<b>Field added. </b>
<code>uint64_t carryover_bytes[2]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int carryover_ios[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>bool has_rules[2]</code>
</li>
</ul>
</details>
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
<code>uint64_t carryover_bytes[2]</code> ➡️ <code>long long int carryover_bytes[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int carryover_ios[2]</code> ➡️ <code>int carryover_ios[2]</code>
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

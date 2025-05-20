# Struct: <code>elevator_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct elevator_ops {
    elevator_merge_fn *elevator_merge_fn;
    elevator_merged_fn *elevator_merged_fn;
    elevator_merge_req_fn *elevator_merge_req_fn;
    elevator_allow_merge_fn *elevator_allow_merge_fn;
    elevator_bio_merged_fn *elevator_bio_merged_fn;
    elevator_dispatch_fn *elevator_dispatch_fn;
    elevator_add_req_fn *elevator_add_req_fn;
    elevator_activate_req_fn *elevator_activate_req_fn;
    elevator_deactivate_req_fn *elevator_deactivate_req_fn;
    elevator_completed_req_fn *elevator_completed_req_fn;
    elevator_request_list_fn *elevator_former_req_fn;
    elevator_request_list_fn *elevator_latter_req_fn;
    elevator_init_icq_fn *elevator_init_icq_fn;
    elevator_exit_icq_fn *elevator_exit_icq_fn;
    elevator_set_req_fn *elevator_set_req_fn;
    elevator_put_req_fn *elevator_put_req_fn;
    elevator_may_queue_fn *elevator_may_queue_fn;
    elevator_init_fn *elevator_init_fn;
    elevator_exit_fn *elevator_exit_fn;
    elevator_registered_fn *elevator_registered_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct elevator_ops {
    elevator_merge_fn *elevator_merge_fn;
    elevator_merged_fn *elevator_merged_fn;
    elevator_merge_req_fn *elevator_merge_req_fn;
    elevator_allow_bio_merge_fn *elevator_allow_bio_merge_fn;
    elevator_allow_rq_merge_fn *elevator_allow_rq_merge_fn;
    elevator_bio_merged_fn *elevator_bio_merged_fn;
    elevator_dispatch_fn *elevator_dispatch_fn;
    elevator_add_req_fn *elevator_add_req_fn;
    elevator_activate_req_fn *elevator_activate_req_fn;
    elevator_deactivate_req_fn *elevator_deactivate_req_fn;
    elevator_completed_req_fn *elevator_completed_req_fn;
    elevator_request_list_fn *elevator_former_req_fn;
    elevator_request_list_fn *elevator_latter_req_fn;
    elevator_init_icq_fn *elevator_init_icq_fn;
    elevator_exit_icq_fn *elevator_exit_icq_fn;
    elevator_set_req_fn *elevator_set_req_fn;
    elevator_put_req_fn *elevator_put_req_fn;
    elevator_may_queue_fn *elevator_may_queue_fn;
    elevator_init_fn *elevator_init_fn;
    elevator_exit_fn *elevator_exit_fn;
    elevator_registered_fn *elevator_registered_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct elevator_ops {
    elevator_merge_fn *elevator_merge_fn;
    elevator_merged_fn *elevator_merged_fn;
    elevator_merge_req_fn *elevator_merge_req_fn;
    elevator_allow_bio_merge_fn *elevator_allow_bio_merge_fn;
    elevator_allow_rq_merge_fn *elevator_allow_rq_merge_fn;
    elevator_bio_merged_fn *elevator_bio_merged_fn;
    elevator_dispatch_fn *elevator_dispatch_fn;
    elevator_add_req_fn *elevator_add_req_fn;
    elevator_activate_req_fn *elevator_activate_req_fn;
    elevator_deactivate_req_fn *elevator_deactivate_req_fn;
    elevator_completed_req_fn *elevator_completed_req_fn;
    elevator_request_list_fn *elevator_former_req_fn;
    elevator_request_list_fn *elevator_latter_req_fn;
    elevator_init_icq_fn *elevator_init_icq_fn;
    elevator_exit_icq_fn *elevator_exit_icq_fn;
    elevator_set_req_fn *elevator_set_req_fn;
    elevator_put_req_fn *elevator_put_req_fn;
    elevator_may_queue_fn *elevator_may_queue_fn;
    elevator_init_fn *elevator_init_fn;
    elevator_exit_fn *elevator_exit_fn;
    elevator_registered_fn *elevator_registered_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct elevator_ops {
    elevator_merge_fn *elevator_merge_fn;
    elevator_merged_fn *elevator_merged_fn;
    elevator_merge_req_fn *elevator_merge_req_fn;
    elevator_allow_bio_merge_fn *elevator_allow_bio_merge_fn;
    elevator_allow_rq_merge_fn *elevator_allow_rq_merge_fn;
    elevator_bio_merged_fn *elevator_bio_merged_fn;
    elevator_dispatch_fn *elevator_dispatch_fn;
    elevator_add_req_fn *elevator_add_req_fn;
    elevator_activate_req_fn *elevator_activate_req_fn;
    elevator_deactivate_req_fn *elevator_deactivate_req_fn;
    elevator_completed_req_fn *elevator_completed_req_fn;
    elevator_request_list_fn *elevator_former_req_fn;
    elevator_request_list_fn *elevator_latter_req_fn;
    elevator_init_icq_fn *elevator_init_icq_fn;
    elevator_exit_icq_fn *elevator_exit_icq_fn;
    elevator_set_req_fn *elevator_set_req_fn;
    elevator_put_req_fn *elevator_put_req_fn;
    elevator_may_queue_fn *elevator_may_queue_fn;
    elevator_init_fn *elevator_init_fn;
    elevator_exit_fn *elevator_exit_fn;
    elevator_registered_fn *elevator_registered_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct elevator_ops {
    elevator_merge_fn *elevator_merge_fn;
    elevator_merged_fn *elevator_merged_fn;
    elevator_merge_req_fn *elevator_merge_req_fn;
    elevator_allow_bio_merge_fn *elevator_allow_bio_merge_fn;
    elevator_allow_rq_merge_fn *elevator_allow_rq_merge_fn;
    elevator_bio_merged_fn *elevator_bio_merged_fn;
    elevator_dispatch_fn *elevator_dispatch_fn;
    elevator_add_req_fn *elevator_add_req_fn;
    elevator_activate_req_fn *elevator_activate_req_fn;
    elevator_deactivate_req_fn *elevator_deactivate_req_fn;
    elevator_completed_req_fn *elevator_completed_req_fn;
    elevator_request_list_fn *elevator_former_req_fn;
    elevator_request_list_fn *elevator_latter_req_fn;
    elevator_init_icq_fn *elevator_init_icq_fn;
    elevator_exit_icq_fn *elevator_exit_icq_fn;
    elevator_set_req_fn *elevator_set_req_fn;
    elevator_put_req_fn *elevator_put_req_fn;
    elevator_may_queue_fn *elevator_may_queue_fn;
    elevator_init_fn *elevator_init_fn;
    elevator_exit_fn *elevator_exit_fn;
    elevator_registered_fn *elevator_registered_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct elevator_ops {
    elevator_merge_fn *elevator_merge_fn;
    elevator_merged_fn *elevator_merged_fn;
    elevator_merge_req_fn *elevator_merge_req_fn;
    elevator_allow_bio_merge_fn *elevator_allow_bio_merge_fn;
    elevator_allow_rq_merge_fn *elevator_allow_rq_merge_fn;
    elevator_bio_merged_fn *elevator_bio_merged_fn;
    elevator_dispatch_fn *elevator_dispatch_fn;
    elevator_add_req_fn *elevator_add_req_fn;
    elevator_activate_req_fn *elevator_activate_req_fn;
    elevator_deactivate_req_fn *elevator_deactivate_req_fn;
    elevator_completed_req_fn *elevator_completed_req_fn;
    elevator_request_list_fn *elevator_former_req_fn;
    elevator_request_list_fn *elevator_latter_req_fn;
    elevator_init_icq_fn *elevator_init_icq_fn;
    elevator_exit_icq_fn *elevator_exit_icq_fn;
    elevator_set_req_fn *elevator_set_req_fn;
    elevator_put_req_fn *elevator_put_req_fn;
    elevator_may_queue_fn *elevator_may_queue_fn;
    elevator_init_fn *elevator_init_fn;
    elevator_exit_fn *elevator_exit_fn;
    elevator_registered_fn *elevator_registered_fn;
};
```
</details>
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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
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
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>elevator_allow_bio_merge_fn *elevator_allow_bio_merge_fn</code>
</li>
<li>
<b>Field added. </b>
<code>elevator_allow_rq_merge_fn *elevator_allow_rq_merge_fn</code>
</li>
<li>
<b>Field removed. </b>
<code>elevator_allow_merge_fn *elevator_allow_merge_fn</code>
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
</ul>

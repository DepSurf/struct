# Struct: <code>scsi_transport_template</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*it_nexus_response)(struct Scsi_Host *, u64, int);
    int (*tsk_mgmt_response)(struct Scsi_Host *, u64, u64, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*it_nexus_response)(struct Scsi_Host *, u64, int);
    int (*tsk_mgmt_response)(struct Scsi_Host *, u64, u64, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*it_nexus_response)(struct Scsi_Host *, u64, int);
    int (*tsk_mgmt_response)(struct Scsi_Host *, u64, u64, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
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
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
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
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct scsi_transport_template {
    struct transport_container host_attrs;
    struct transport_container target_attrs;
    struct transport_container device_attrs;
    int (*user_scan)(struct Scsi_Host *, uint, uint, u64);
    int device_size;
    int device_private_offset;
    int target_size;
    int target_private_offset;
    int host_size;
    unsigned int create_work_queue;
    void (*eh_strategy_handler)(struct Scsi_Host *);
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
<b>Field removed. </b>
<code>enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*it_nexus_response)(struct Scsi_Host *, u64, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*tsk_mgmt_response)(struct Scsi_Host *, u64, u64, int)</code>
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

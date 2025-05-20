# Struct: <code>taskstats</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
    __u64 compact_count;
    __u64 compact_delay_total;
    __u32 ac_tgid;
    __u64 ac_tgetime;
    __u64 ac_exe_dev;
    __u64 ac_exe_inode;
    __u64 wpcopy_count;
    __u64 wpcopy_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
    __u64 compact_count;
    __u64 compact_delay_total;
    __u32 ac_tgid;
    __u64 ac_tgetime;
    __u64 ac_exe_dev;
    __u64 ac_exe_inode;
    __u64 wpcopy_count;
    __u64 wpcopy_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
    __u64 compact_count;
    __u64 compact_delay_total;
    __u32 ac_tgid;
    __u64 ac_tgetime;
    __u64 ac_exe_dev;
    __u64 ac_exe_inode;
    __u64 wpcopy_count;
    __u64 wpcopy_delay_total;
    __u64 irq_count;
    __u64 irq_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
    __u64 ac_btime64;
    __u64 compact_count;
    __u64 compact_delay_total;
    __u32 ac_tgid;
    __u64 ac_tgetime;
    __u64 ac_exe_dev;
    __u64 ac_exe_inode;
    __u64 wpcopy_count;
    __u64 wpcopy_delay_total;
    __u64 irq_count;
    __u64 irq_delay_total;
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
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
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
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct taskstats {
    __u16 version;
    __u32 ac_exitcode;
    __u8 ac_flag;
    __u8 ac_nice;
    __u64 cpu_count;
    __u64 cpu_delay_total;
    __u64 blkio_count;
    __u64 blkio_delay_total;
    __u64 swapin_count;
    __u64 swapin_delay_total;
    __u64 cpu_run_real_total;
    __u64 cpu_run_virtual_total;
    char ac_comm[32];
    __u8 ac_sched;
    __u8 ac_pad[3];
    __u32 ac_uid;
    __u32 ac_gid;
    __u32 ac_pid;
    __u32 ac_ppid;
    __u32 ac_btime;
    __u64 ac_etime;
    __u64 ac_utime;
    __u64 ac_stime;
    __u64 ac_minflt;
    __u64 ac_majflt;
    __u64 coremem;
    __u64 virtmem;
    __u64 hiwater_rss;
    __u64 hiwater_vm;
    __u64 read_char;
    __u64 write_char;
    __u64 read_syscalls;
    __u64 write_syscalls;
    __u64 read_bytes;
    __u64 write_bytes;
    __u64 cancelled_write_bytes;
    __u64 nvcsw;
    __u64 nivcsw;
    __u64 ac_utimescaled;
    __u64 ac_stimescaled;
    __u64 cpu_scaled_run_real_total;
    __u64 freepages_count;
    __u64 freepages_delay_total;
    __u64 thrashing_count;
    __u64 thrashing_delay_total;
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
<code>__u64 thrashing_count</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 thrashing_delay_total</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 ac_btime64</code>
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 compact_count</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 compact_delay_total</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 ac_tgid</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 ac_tgetime</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 ac_exe_dev</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 ac_exe_inode</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 wpcopy_count</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 wpcopy_delay_total</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 irq_count</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 irq_delay_total</code>
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

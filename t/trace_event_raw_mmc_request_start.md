# Struct: <code>trace_event_raw_mmc_request_start</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blksz;
    unsigned int data_flags;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blksz;
    unsigned int data_flags;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blksz;
    unsigned int data_flags;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
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
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
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
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_event_raw_mmc_request_start {
    struct trace_entry ent;
    u32 cmd_opcode;
    u32 cmd_arg;
    unsigned int cmd_flags;
    unsigned int cmd_retries;
    u32 stop_opcode;
    u32 stop_arg;
    unsigned int stop_flags;
    unsigned int stop_retries;
    u32 sbc_opcode;
    u32 sbc_arg;
    unsigned int sbc_flags;
    unsigned int sbc_retries;
    unsigned int blocks;
    unsigned int blk_addr;
    unsigned int blksz;
    unsigned int data_flags;
    int tag;
    unsigned int can_retune;
    unsigned int doing_retune;
    unsigned int retune_now;
    int need_retune;
    int hold_retune;
    unsigned int retune_period;
    struct mmc_request *mrq;
    u32 __data_loc_name;
    char __data[0];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int blk_addr</code>
</li>
<li>
<b>Field added. </b>
<code>int tag</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

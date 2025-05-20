# Struct: <code>trace_event_raw_mmc_request_done</code>

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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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
struct trace_event_raw_mmc_request_done {
    struct trace_entry ent;
    u32 cmd_opcode;
    int cmd_err;
    u32 cmd_resp[4];
    unsigned int cmd_retries;
    u32 stop_opcode;
    int stop_err;
    u32 stop_resp[4];
    unsigned int stop_retries;
    u32 sbc_opcode;
    int sbc_err;
    u32 sbc_resp[4];
    unsigned int sbc_retries;
    unsigned int bytes_xfered;
    int data_err;
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

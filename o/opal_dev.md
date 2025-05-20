# Struct: <code>opal_dev</code>

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
struct opal_dev {
    bool supported;
    void *data;
    sec_send_recv *send_recv;
    const struct opal_step *steps;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    const struct opal_step *steps;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    const struct opal_step *steps;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    const struct opal_step *steps;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct opal_dev {
    u32 flags;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 *cmd;
    u8 *resp;
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct opal_dev {
    u32 flags;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    u32 logical_block_size;
    u8 align_required;
    size_t pos;
    u8 *cmd;
    u8 *resp;
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct opal_dev {
    u32 flags;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    u32 logical_block_size;
    u8 align_required;
    size_t pos;
    u8 *cmd;
    u8 *resp;
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
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
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
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
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct opal_dev {
    bool supported;
    bool mbr_enabled;
    void *data;
    sec_send_recv *send_recv;
    struct mutex dev_lock;
    u16 comid;
    u32 hsn;
    u32 tsn;
    u64 align;
    u64 lowest_lba;
    size_t pos;
    u8 cmd[2048];
    u8 resp[2048];
    struct parsed_resp parsed;
    size_t prev_d_len;
    void *prev_data;
    struct list_head unlk_lst;
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool mbr_enabled</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const struct opal_step *steps</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>bool supported</code>
</li>
<li>
<b>Field removed. </b>
<code>bool mbr_enabled</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 cmd[2048]</code> ➡️ <code>u8 *cmd</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 resp[2048]</code> ➡️ <code>u8 *resp</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 logical_block_size</code>
</li>
<li>
<b>Field added. </b>
<code>u8 align_required</code>
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

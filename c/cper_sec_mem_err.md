# Struct: <code>cper_sec_mem_err</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    __u64 validation_bits;
    __u64 error_status;
    __u64 physical_addr;
    __u64 physical_addr_mask;
    __u16 node;
    __u16 card;
    __u16 module;
    __u16 bank;
    __u16 device;
    __u16 row;
    __u16 column;
    __u16 bit_pos;
    __u64 requestor_id;
    __u64 responder_id;
    __u64 target_id;
    __u8 error_type;
    __u8 reserved;
    __u16 rank;
    __u16 mem_array_handle;
    __u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 extended;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
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
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cper_sec_mem_err {
    u64 validation_bits;
    u64 error_status;
    u64 physical_addr;
    u64 physical_addr_mask;
    u16 node;
    u16 card;
    u16 module;
    u16 bank;
    u16 device;
    u16 row;
    u16 column;
    u16 bit_pos;
    u64 requestor_id;
    u64 responder_id;
    u64 target_id;
    u8 error_type;
    u8 reserved;
    u16 rank;
    u16 mem_array_handle;
    u16 mem_dev_handle;
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__u64 validation_bits</code> ➡️ <code>u64 validation_bits</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 error_status</code> ➡️ <code>u64 error_status</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 physical_addr</code> ➡️ <code>u64 physical_addr</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 physical_addr_mask</code> ➡️ <code>u64 physical_addr_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 node</code> ➡️ <code>u16 node</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 card</code> ➡️ <code>u16 card</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 module</code> ➡️ <code>u16 module</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 bank</code> ➡️ <code>u16 bank</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 device</code> ➡️ <code>u16 device</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 row</code> ➡️ <code>u16 row</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 column</code> ➡️ <code>u16 column</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 bit_pos</code> ➡️ <code>u16 bit_pos</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 requestor_id</code> ➡️ <code>u64 requestor_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 responder_id</code> ➡️ <code>u64 responder_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 target_id</code> ➡️ <code>u64 target_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 error_type</code> ➡️ <code>u8 error_type</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 reserved</code> ➡️ <code>u8 reserved</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 rank</code> ➡️ <code>u16 rank</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 mem_array_handle</code> ➡️ <code>u16 mem_array_handle</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 mem_dev_handle</code> ➡️ <code>u16 mem_dev_handle</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 extended</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved</code>
</li>
</ul>
</details>
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
</ul>
<b>Flavor</b>
<ul>
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

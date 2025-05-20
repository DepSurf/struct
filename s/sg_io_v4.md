# Struct: <code>sg_io_v4</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
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
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
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
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sg_io_v4 {
    __s32 guard;
    __u32 protocol;
    __u32 subprotocol;
    __u32 request_len;
    __u64 request;
    __u64 request_tag;
    __u32 request_attr;
    __u32 request_priority;
    __u32 request_extra;
    __u32 max_response_len;
    __u64 response;
    __u32 dout_iovec_count;
    __u32 dout_xfer_len;
    __u32 din_iovec_count;
    __u32 din_xfer_len;
    __u64 dout_xferp;
    __u64 din_xferp;
    __u32 timeout;
    __u32 flags;
    __u64 usr_ptr;
    __u32 spare_in;
    __u32 driver_status;
    __u32 transport_status;
    __u32 device_status;
    __u32 retry_delay;
    __u32 info;
    __u32 duration;
    __u32 response_len;
    __s32 din_resid;
    __s32 dout_resid;
    __u64 generated_tag;
    __u32 spare_out;
    __u32 padding;
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

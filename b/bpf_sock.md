# Struct: <code>bpf_sock</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __be16 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __be16 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __be16 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __be16 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
    __s32 rx_queue_mapping;
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
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
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
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_sock {
    __u32 bound_dev_if;
    __u32 family;
    __u32 type;
    __u32 protocol;
    __u32 mark;
    __u32 priority;
    __u32 src_ip4;
    __u32 src_ip6[4];
    __u32 src_port;
    __u32 dst_port;
    __u32 dst_ip4;
    __u32 dst_ip6[4];
    __u32 state;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 dst_port</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 dst_ip4</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 dst_ip6[4]</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 state</code>
</li>
</ul>
</details>
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
<code>__s32 rx_queue_mapping</code>
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
<b>Field type changed. </b>
<code>__u32 dst_port</code> ➡️ <code>__be16 dst_port</code>
</li>
</ul>
</details>
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

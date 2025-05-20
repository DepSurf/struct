# Struct: <code>nf_tcp_net</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nf_tcp_net {
    struct nf_proto_net pn;
    unsigned int timeouts[14];
    unsigned int tcp_loose;
    unsigned int tcp_be_liberal;
    unsigned int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    u8 tcp_loose;
    u8 tcp_be_liberal;
    u8 tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    u8 tcp_loose;
    u8 tcp_be_liberal;
    u8 tcp_max_retrans;
    u8 tcp_ignore_invalid_rst;
    unsigned int offload_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    u8 tcp_loose;
    u8 tcp_be_liberal;
    u8 tcp_max_retrans;
    u8 tcp_ignore_invalid_rst;
    unsigned int offload_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    u8 tcp_loose;
    u8 tcp_be_liberal;
    u8 tcp_max_retrans;
    u8 tcp_ignore_invalid_rst;
    unsigned int offload_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    u8 tcp_loose;
    u8 tcp_be_liberal;
    u8 tcp_max_retrans;
    u8 tcp_ignore_invalid_rst;
    unsigned int offload_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    u8 tcp_loose;
    u8 tcp_be_liberal;
    u8 tcp_max_retrans;
    u8 tcp_ignore_invalid_rst;
    unsigned int offload_timeout;
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
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
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
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nf_tcp_net {
    unsigned int timeouts[14];
    int tcp_loose;
    int tcp_be_liberal;
    int tcp_max_retrans;
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
<b>Field removed. </b>
<code>struct nf_proto_net pn</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int tcp_loose</code> ➡️ <code>int tcp_loose</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int tcp_be_liberal</code> ➡️ <code>int tcp_be_liberal</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int tcp_max_retrans</code> ➡️ <code>int tcp_max_retrans</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int tcp_loose</code> ➡️ <code>u8 tcp_loose</code>
</li>
<li>
<b>Field type changed. </b>
<code>int tcp_be_liberal</code> ➡️ <code>u8 tcp_be_liberal</code>
</li>
<li>
<b>Field type changed. </b>
<code>int tcp_max_retrans</code> ➡️ <code>u8 tcp_max_retrans</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 tcp_ignore_invalid_rst</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int offload_timeout</code>
</li>
</ul>
</details>
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

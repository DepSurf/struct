# Struct: <code>sock_reuseport</code>

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
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    bool bind_inany;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    u16 num_closed_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    u16 num_closed_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    u16 num_closed_socks;
    u16 incoming_cpu;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    u16 num_closed_socks;
    u16 incoming_cpu;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    u16 num_closed_socks;
    u16 incoming_cpu;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
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
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
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
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sock_reuseport {
    struct callback_head rcu;
    u16 max_socks;
    u16 num_socks;
    unsigned int synq_overflow_ts;
    unsigned int reuseport_id;
    unsigned int bind_inany;
    unsigned int has_conns;
    struct bpf_prog *prog;
    struct sock * socks[0];
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
<code>unsigned int synq_overflow_ts</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int reuseport_id</code>
</li>
<li>
<b>Field added. </b>
<code>bool bind_inany</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int has_conns</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool bind_inany</code> ➡️ <code>unsigned int bind_inany</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 num_closed_socks</code>
</li>
</ul>
</details>
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
<code>u16 incoming_cpu</code>
</li>
</ul>
</details>
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

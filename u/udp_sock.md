# Struct: <code>udp_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    __u16 len;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    __u16 len;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    __u16 len;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    __u16 len;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    __u16 len;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    unsigned char accept_udp_l4;
    unsigned char accept_udp_fraglist;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    unsigned char accept_udp_l4;
    unsigned char accept_udp_fraglist;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    unsigned char accept_udp_l4;
    unsigned char accept_udp_fraglist;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    unsigned char accept_udp_l4;
    unsigned char accept_udp_fraglist;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_err_rcv)(struct sock *, struct sk_buff *, int, __be16, u32, u8 *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
    int forward_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    unsigned char accept_udp_l4;
    unsigned char accept_udp_fraglist;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_err_rcv)(struct sock *, struct sk_buff *, int, __be16, u32, u8 *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
    int forward_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    long unsigned int udp_flags;
    int pending;
    __u8 encap_type;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    void (*encap_err_rcv)(struct sock *, struct sk_buff *, int, __be16, u32, u8 *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
    int forward_threshold;
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
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
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
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct udp_sock {
    struct inet_sock inet;
    int pending;
    unsigned int corkflag;
    __u8 encap_type;
    unsigned char no_check6_tx;
    unsigned char no_check6_rx;
    unsigned char encap_enabled;
    unsigned char gro_enabled;
    __u16 len;
    __u16 gso_size;
    __u16 pcslen;
    __u16 pcrlen;
    __u8 pcflag;
    __u8 unused[3];
    int (*encap_rcv)(struct sock *, struct sk_buff *);
    int (*encap_err_lookup)(struct sock *, struct sk_buff *);
    void (*encap_destroy)(struct sock *);
    struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *);
    int (*gro_complete)(struct sock *, struct sk_buff *, int);
    struct sk_buff_head reader_queue;
    int forward_deficit;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*gro_complete)(struct sock *, struct sk_buff *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int forward_deficit</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff_head reader_queue</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u16 gso_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char encap_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char gro_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>int (*encap_err_lookup)(struct sock *, struct sk_buff *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sk_buff ** (*gro_receive)(struct sock *, struct sk_buff **, struct sk_buff *)</code> ➡️ <code>struct sk_buff * (*gro_receive)(struct sock *, struct list_head *, struct sk_buff *)</code>
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
<b>Field added. </b>
<code>unsigned char accept_udp_l4</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char accept_udp_fraglist</code>
</li>
</ul>
</details>
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
<code>void (*encap_err_rcv)(struct sock *, struct sk_buff *, int, __be16, u32, u8 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int forward_threshold</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int udp_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int corkflag</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char no_check6_tx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char no_check6_rx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char encap_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char gro_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char accept_udp_l4</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char accept_udp_fraglist</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 pcflag</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 unused[3]</code>
</li>
</ul>
</details>
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

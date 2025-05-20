# Struct: <code>cfg80211_wowlan_tcp</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
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
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
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
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cfg80211_wowlan_tcp {
    struct socket *sock;
    __be32 src;
    __be32 dst;
    u16 src_port;
    u16 dst_port;
    u8 dst_mac[6];
    int payload_len;
    const u8 *payload;
    struct nl80211_wowlan_tcp_data_seq payload_seq;
    u32 data_interval;
    u32 wake_len;
    const u8 *wake_data;
    const u8 *wake_mask;
    u32 tokens_size;
    struct nl80211_wowlan_tcp_data_token payload_tok;
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

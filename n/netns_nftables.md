# Struct: <code>netns_nftables</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head af_info;
    struct list_head commit_list;
    struct nft_af_info *ipv4;
    struct nft_af_info *ipv6;
    struct nft_af_info *inet;
    struct nft_af_info *arp;
    struct nft_af_info *bridge;
    struct nft_af_info *netdev;
    unsigned int base_seq;
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head af_info;
    struct list_head commit_list;
    struct nft_af_info *ipv4;
    struct nft_af_info *ipv6;
    struct nft_af_info *inet;
    struct nft_af_info *arp;
    struct nft_af_info *bridge;
    struct nft_af_info *netdev;
    unsigned int base_seq;
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head af_info;
    struct list_head commit_list;
    struct nft_af_info *ipv4;
    struct nft_af_info *ipv6;
    struct nft_af_info *inet;
    struct nft_af_info *arp;
    struct nft_af_info *bridge;
    struct nft_af_info *netdev;
    unsigned int base_seq;
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head af_info;
    struct list_head commit_list;
    struct nft_af_info *ipv4;
    struct nft_af_info *ipv6;
    struct nft_af_info *inet;
    struct nft_af_info *arp;
    struct nft_af_info *bridge;
    struct nft_af_info *netdev;
    unsigned int base_seq;
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head af_info;
    struct list_head commit_list;
    struct nft_af_info *ipv4;
    struct nft_af_info *ipv6;
    struct nft_af_info *inet;
    struct nft_af_info *arp;
    struct nft_af_info *bridge;
    struct nft_af_info *netdev;
    unsigned int base_seq;
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct list_head notify_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_nftables {
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_nftables {
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_nftables {
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_nftables {
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_nftables {
    u8 gencursor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_nftables {
    u8 gencursor;
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
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
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
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_nftables {
    struct list_head tables;
    struct list_head commit_list;
    struct list_head module_list;
    struct mutex commit_mutex;
    unsigned int base_seq;
    u8 gencursor;
    u8 validate_state;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head tables</code>
</li>
<li>
<b>Field added. </b>
<code>u8 validate_state</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head af_info</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nft_af_info *ipv4</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nft_af_info *ipv6</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nft_af_info *inet</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nft_af_info *arp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nft_af_info *bridge</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nft_af_info *netdev</code>
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
<code>struct mutex commit_mutex</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head module_list</code>
</li>
</ul>
</details>
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
<code>struct list_head notify_list</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head tables</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head commit_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head module_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head notify_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex commit_mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int base_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 validate_state</code>
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

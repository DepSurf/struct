# Struct: <code>netns_nf</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct list_head hooks[104];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct list_head hooks[104];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entry * hooks[104];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entry * hooks[104];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks[104];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    unsigned int defrag_ipv4_users;
    unsigned int defrag_ipv6_users;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    unsigned int defrag_ipv4_users;
    unsigned int defrag_ipv6_users;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_logger * nf_loggers[11];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    unsigned int defrag_ipv4_users;
    unsigned int defrag_ipv6_users;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_logger * nf_loggers[11];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    unsigned int defrag_ipv4_users;
    unsigned int defrag_ipv6_users;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_logger * nf_loggers[11];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    unsigned int defrag_ipv4_users;
    unsigned int defrag_ipv6_users;
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
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
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
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_nf {
    struct proc_dir_entry *proc_netfilter;
    const struct nf_queue_handler *queue_handler;
    const struct nf_logger * nf_loggers[13];
    struct ctl_table_header *nf_log_dir_header;
    struct nf_hook_entries * hooks_ipv4[5];
    struct nf_hook_entries * hooks_ipv6[5];
    struct nf_hook_entries * hooks_arp[3];
    struct nf_hook_entries * hooks_bridge[5];
    struct nf_hook_entries * hooks_decnet[7];
    bool defrag_ipv4;
    bool defrag_ipv6;
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
<code>const struct nf_queue_handler *queue_handler</code>
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
<code>bool defrag_ipv4</code>
</li>
<li>
<b>Field added. </b>
<code>bool defrag_ipv6</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head hooks[104]</code> ➡️ <code>struct nf_hook_entry * hooks[104]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct nf_hook_entry * hooks[104]</code> ➡️ <code>struct nf_hook_entries * hooks[104]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct nf_hook_entries * hooks_ipv4[5]</code>
</li>
<li>
<b>Field added. </b>
<code>struct nf_hook_entries * hooks_ipv6[5]</code>
</li>
<li>
<b>Field added. </b>
<code>struct nf_hook_entries * hooks_arp[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct nf_hook_entries * hooks_bridge[5]</code>
</li>
<li>
<b>Field added. </b>
<code>struct nf_hook_entries * hooks_decnet[7]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nf_hook_entries * hooks[104]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool defrag_ipv4</code>
</li>
<li>
<b>Field removed. </b>
<code>bool defrag_ipv6</code>
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
<code>unsigned int defrag_ipv4_users</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int defrag_ipv6_users</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct nf_queue_handler *queue_handler</code>
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
<b>Field removed. </b>
<code>struct nf_hook_entries * hooks_decnet[7]</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct nf_logger * nf_loggers[13]</code> ➡️ <code>const struct nf_logger * nf_loggers[11]</code>
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

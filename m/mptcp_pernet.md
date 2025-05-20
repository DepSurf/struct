# Struct: <code>mptcp_pernet</code>

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
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    int mptcp_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    int mptcp_enabled;
    unsigned int add_addr_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    int mptcp_enabled;
    unsigned int add_addr_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    unsigned int add_addr_timeout;
    unsigned int stale_loss_cnt;
    u8 mptcp_enabled;
    u8 checksum_enabled;
    u8 allow_join_initial_addr_port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    unsigned int add_addr_timeout;
    unsigned int stale_loss_cnt;
    u8 mptcp_enabled;
    u8 checksum_enabled;
    u8 allow_join_initial_addr_port;
    u8 pm_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    unsigned int add_addr_timeout;
    unsigned int stale_loss_cnt;
    u8 mptcp_enabled;
    u8 checksum_enabled;
    u8 allow_join_initial_addr_port;
    u8 pm_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    unsigned int add_addr_timeout;
    unsigned int stale_loss_cnt;
    u8 mptcp_enabled;
    u8 checksum_enabled;
    u8 allow_join_initial_addr_port;
    u8 pm_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_pernet {
    struct ctl_table_header *ctl_table_hdr;
    unsigned int add_addr_timeout;
    unsigned int close_timeout;
    unsigned int stale_loss_cnt;
    u8 mptcp_enabled;
    u8 checksum_enabled;
    u8 allow_join_initial_addr_port;
    u8 pm_type;
    char scheduler[16];
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
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
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int add_addr_timeout</code>
</li>
</ul>
</details>
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
<code>unsigned int stale_loss_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>u8 checksum_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u8 allow_join_initial_addr_port</code>
</li>
<li>
<b>Field type changed. </b>
<code>int mptcp_enabled</code> ➡️ <code>u8 mptcp_enabled</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 pm_type</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int close_timeout</code>
</li>
<li>
<b>Field added. </b>
<code>char scheduler[16]</code>
</li>
</ul>
</details>
</li>
</ul>

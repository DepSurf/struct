# Struct: <code>mptcp_data_frag</code>

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
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    int data_len;
    int offset;
    int overhead;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_data_frag {
    struct list_head list;
    u64 data_seq;
    u16 data_len;
    u16 offset;
    u16 overhead;
    u16 already_sent;
    struct page *page;
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
<code>u16 already_sent</code>
</li>
<li>
<b>Field type changed. </b>
<code>int data_len</code> ➡️ <code>u16 data_len</code>
</li>
<li>
<b>Field type changed. </b>
<code>int offset</code> ➡️ <code>u16 offset</code>
</li>
<li>
<b>Field type changed. </b>
<code>int overhead</code> ➡️ <code>u16 overhead</code>
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

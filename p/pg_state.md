# Struct: <code>pg_state</code>

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
struct pg_state {
    int level;
    pgprot_t current_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pg_state {
    struct ptdump_state ptdump;
    int level;
    pgprotval_t current_prot;
    pgprotval_t effective_prot;
    pgprotval_t prot_levels[5];
    long unsigned int start_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
    struct seq_file *seq;
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
struct pg_state {
    struct seq_file *seq;
    const struct addr_marker *marker;
    long unsigned int start_address;
    unsigned int level;
    u64 current_prot;
    bool check_wx;
    long unsigned int wx_pages;
    long unsigned int uxn_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pg_state {
    struct seq_file *seq;
    const struct addr_marker *marker;
    long unsigned int start_address;
    unsigned int level;
    u64 current_prot;
    bool check_wx;
    long unsigned int wx_pages;
    const char *current_domain;
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pg_state {
    int level;
    pgprot_t current_prot;
    pgprotval_t effective_prot;
    long unsigned int start_address;
    long unsigned int current_address;
    const struct addr_marker *marker;
    long unsigned int lines;
    bool to_dmesg;
    bool check_wx;
    long unsigned int wx_pages;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>pgprotval_t effective_prot</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ptdump_state ptdump</code>
</li>
<li>
<b>Field added. </b>
<code>pgprotval_t prot_levels[5]</code>
</li>
<li>
<b>Field added. </b>
<code>struct seq_file *seq</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int current_address</code>
</li>
<li>
<b>Field type changed. </b>
<code>pgprot_t current_prot</code> ➡️ <code>pgprotval_t current_prot</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct seq_file *seq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int uxn_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>pgprotval_t effective_prot</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int current_address</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int lines</code>
</li>
<li>
<b>Field removed. </b>
<code>bool to_dmesg</code>
</li>
<li>
<b>Field type changed. </b>
<code>int level</code> ➡️ <code>unsigned int level</code>
</li>
<li>
<b>Field type changed. </b>
<code>pgprot_t current_prot</code> ➡️ <code>u64 current_prot</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct seq_file *seq</code>
</li>
<li>
<b>Field added. </b>
<code>const char *current_domain</code>
</li>
<li>
<b>Field removed. </b>
<code>pgprotval_t effective_prot</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int current_address</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int lines</code>
</li>
<li>
<b>Field removed. </b>
<code>bool to_dmesg</code>
</li>
<li>
<b>Field type changed. </b>
<code>int level</code> ➡️ <code>unsigned int level</code>
</li>
<li>
<b>Field type changed. </b>
<code>pgprot_t current_prot</code> ➡️ <code>u64 current_prot</code>
</li>
</ul>
</details>
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

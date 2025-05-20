# Struct: <code>mmc_ioc_cmd</code>

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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct mmc_ioc_cmd {
    int write_flag;
    int is_acmd;
    __u32 opcode;
    __u32 arg;
    __u32 response[4];
    unsigned int flags;
    unsigned int blksz;
    unsigned int blocks;
    unsigned int postsleep_min_us;
    unsigned int postsleep_max_us;
    unsigned int data_timeout_ns;
    unsigned int cmd_timeout_ms;
    __u32 __pad;
    __u64 data_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_ioc_cmd {
    int write_flag;
    int is_acmd;
    __u32 opcode;
    __u32 arg;
    __u32 response[4];
    unsigned int flags;
    unsigned int blksz;
    unsigned int blocks;
    unsigned int postsleep_min_us;
    unsigned int postsleep_max_us;
    unsigned int data_timeout_ns;
    unsigned int cmd_timeout_ms;
    __u32 __pad;
    __u64 data_ptr;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_ioc_cmd {
    int write_flag;
    int is_acmd;
    __u32 opcode;
    __u32 arg;
    __u32 response[4];
    unsigned int flags;
    unsigned int blksz;
    unsigned int blocks;
    unsigned int postsleep_min_us;
    unsigned int postsleep_max_us;
    unsigned int data_timeout_ns;
    unsigned int cmd_timeout_ms;
    __u32 __pad;
    __u64 data_ptr;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>

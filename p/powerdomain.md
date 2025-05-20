# Struct: <code>powerdomain</code>

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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct powerdomain {
    const char *name;
    union (anon) voltdm;
    const s16 prcm_offs;
    const u8 pwrsts;
    const u8 pwrsts_logic_ret;
    const u8 flags;
    const u8 banks;
    const const u8[5] pwrsts_mem_ret;
    const const u8[5] pwrsts_mem_on;
    const u8 prcm_partition;
    struct clockdomain * pwrdm_clkdms[11];
    struct list_head node;
    struct list_head voltdm_node;
    int state;
    unsigned int state_counter[4];
    unsigned int ret_logic_off_counter;
    unsigned int ret_mem_off_counter[5];
    spinlock_t _lock;
    long unsigned int _lock_flags;
    const u8 pwrstctrl_offs;
    const u8 pwrstst_offs;
    const u32 logicretstate_mask;
    const const u32[5] mem_on_mask;
    const const u32[5] mem_ret_mask;
    const const u32[5] mem_pwrst_mask;
    const const u32[5] mem_retst_mask;
    s64 timer;
    s64 state_timer[4];
    u32 context;
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

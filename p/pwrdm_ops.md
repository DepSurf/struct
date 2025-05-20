# Struct: <code>pwrdm_ops</code>

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
struct pwrdm_ops {
    int (*pwrdm_set_next_pwrst)(struct powerdomain *, u8);
    int (*pwrdm_read_next_pwrst)(struct powerdomain *);
    int (*pwrdm_read_pwrst)(struct powerdomain *);
    int (*pwrdm_read_prev_pwrst)(struct powerdomain *);
    int (*pwrdm_set_logic_retst)(struct powerdomain *, u8);
    int (*pwrdm_set_mem_onst)(struct powerdomain *, u8, u8);
    int (*pwrdm_set_mem_retst)(struct powerdomain *, u8, u8);
    int (*pwrdm_read_logic_pwrst)(struct powerdomain *);
    int (*pwrdm_read_prev_logic_pwrst)(struct powerdomain *);
    int (*pwrdm_read_logic_retst)(struct powerdomain *);
    int (*pwrdm_read_mem_pwrst)(struct powerdomain *, u8);
    int (*pwrdm_read_prev_mem_pwrst)(struct powerdomain *, u8);
    int (*pwrdm_read_mem_retst)(struct powerdomain *, u8);
    int (*pwrdm_clear_all_prev_pwrst)(struct powerdomain *);
    int (*pwrdm_enable_hdwr_sar)(struct powerdomain *);
    int (*pwrdm_disable_hdwr_sar)(struct powerdomain *);
    int (*pwrdm_set_lowpwrstchange)(struct powerdomain *);
    int (*pwrdm_wait_transition)(struct powerdomain *);
    int (*pwrdm_has_voltdm)();
    void (*pwrdm_save_context)(struct powerdomain *);
    void (*pwrdm_restore_context)(struct powerdomain *);
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

# Struct: <code>vcap_rule_internal</code>

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
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vcap_rule_internal {
    struct vcap_rule data;
    struct list_head list;
    struct vcap_admin *admin;
    struct net_device *ndev;
    struct vcap_control *vctrl;
    u32 sort_key;
    int keyset_sw;
    int actionset_sw;
    int keyset_sw_regs;
    int actionset_sw_regs;
    int size;
    u32 addr;
    u32 counter_id;
    struct vcap_counter counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vcap_rule_internal {
    struct vcap_rule data;
    struct list_head list;
    struct vcap_admin *admin;
    struct net_device *ndev;
    struct vcap_control *vctrl;
    u32 sort_key;
    int keyset_sw;
    int actionset_sw;
    int keyset_sw_regs;
    int actionset_sw_regs;
    int size;
    u32 addr;
    u32 counter_id;
    struct vcap_counter counter;
    enum vcap_rule_state state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vcap_rule_internal {
    struct vcap_rule data;
    struct list_head list;
    struct vcap_admin *admin;
    struct net_device *ndev;
    struct vcap_control *vctrl;
    u32 sort_key;
    int keyset_sw;
    int actionset_sw;
    int keyset_sw_regs;
    int actionset_sw_regs;
    int size;
    u32 addr;
    u32 counter_id;
    struct vcap_counter counter;
    enum vcap_rule_state state;
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
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum vcap_rule_state state</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

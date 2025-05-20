# Struct: <code>vcap_info</code>

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
struct vcap_info {
    char *name;
    u16 rows;
    u16 sw_count;
    u16 sw_width;
    u16 sticky_width;
    u16 act_width;
    u16 default_cnt;
    u16 require_cnt_dis;
    u16 version;
    const struct vcap_set *keyfield_set;
    int keyfield_set_size;
    const struct vcap_set *actionfield_set;
    int actionfield_set_size;
    const struct vcap_field **keyfield_set_map;
    int *keyfield_set_map_size;
    const struct vcap_field **actionfield_set_map;
    int *actionfield_set_map_size;
    const struct vcap_typegroup **keyfield_set_typegroups;
    const struct vcap_typegroup **actionfield_set_typegroups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vcap_info {
    char *name;
    u16 rows;
    u16 sw_count;
    u16 sw_width;
    u16 sticky_width;
    u16 act_width;
    u16 default_cnt;
    u16 require_cnt_dis;
    u16 version;
    const struct vcap_set *keyfield_set;
    int keyfield_set_size;
    const struct vcap_set *actionfield_set;
    int actionfield_set_size;
    const struct vcap_field **keyfield_set_map;
    int *keyfield_set_map_size;
    const struct vcap_field **actionfield_set_map;
    int *actionfield_set_map_size;
    const struct vcap_typegroup **keyfield_set_typegroups;
    const struct vcap_typegroup **actionfield_set_typegroups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vcap_info {
    char *name;
    u16 rows;
    u16 sw_count;
    u16 sw_width;
    u16 sticky_width;
    u16 act_width;
    u16 default_cnt;
    u16 require_cnt_dis;
    u16 version;
    const struct vcap_set *keyfield_set;
    int keyfield_set_size;
    const struct vcap_set *actionfield_set;
    int actionfield_set_size;
    const struct vcap_field **keyfield_set_map;
    int *keyfield_set_map_size;
    const struct vcap_field **actionfield_set_map;
    int *actionfield_set_map_size;
    const struct vcap_typegroup **keyfield_set_typegroups;
    const struct vcap_typegroup **actionfield_set_typegroups;
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

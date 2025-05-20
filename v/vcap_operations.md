# Struct: <code>vcap_operations</code>

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
struct vcap_operations {
    enum vcap_keyfield_set (*validate_keyset)(struct net_device *, struct vcap_admin *, struct vcap_rule *, struct vcap_keyset_list *, u16);
    void (*add_default_fields)(struct net_device *, struct vcap_admin *, struct vcap_rule *);
    void (*cache_erase)(struct vcap_admin *);
    void (*cache_write)(struct net_device *, struct vcap_admin *, enum vcap_selection, u32, u32);
    void (*cache_read)(struct net_device *, struct vcap_admin *, enum vcap_selection, u32, u32);
    void (*init)(struct net_device *, struct vcap_admin *, u32, u32);
    void (*update)(struct net_device *, struct vcap_admin *, enum vcap_command, enum vcap_selection, u32);
    void (*move)(struct net_device *, struct vcap_admin *, u32, int, int);
    int (*port_info)(struct net_device *, struct vcap_admin *, struct vcap_output_print *);
    int (*enable)(struct net_device *, struct vcap_admin *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vcap_operations {
    enum vcap_keyfield_set (*validate_keyset)(struct net_device *, struct vcap_admin *, struct vcap_rule *, struct vcap_keyset_list *, u16);
    void (*add_default_fields)(struct net_device *, struct vcap_admin *, struct vcap_rule *);
    void (*cache_erase)(struct vcap_admin *);
    void (*cache_write)(struct net_device *, struct vcap_admin *, enum vcap_selection, u32, u32);
    void (*cache_read)(struct net_device *, struct vcap_admin *, enum vcap_selection, u32, u32);
    void (*init)(struct net_device *, struct vcap_admin *, u32, u32);
    void (*update)(struct net_device *, struct vcap_admin *, enum vcap_command, enum vcap_selection, u32);
    void (*move)(struct net_device *, struct vcap_admin *, u32, int, int);
    int (*port_info)(struct net_device *, struct vcap_admin *, struct vcap_output_print *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vcap_operations {
    enum vcap_keyfield_set (*validate_keyset)(struct net_device *, struct vcap_admin *, struct vcap_rule *, struct vcap_keyset_list *, u16);
    void (*add_default_fields)(struct net_device *, struct vcap_admin *, struct vcap_rule *);
    void (*cache_erase)(struct vcap_admin *);
    void (*cache_write)(struct net_device *, struct vcap_admin *, enum vcap_selection, u32, u32);
    void (*cache_read)(struct net_device *, struct vcap_admin *, enum vcap_selection, u32, u32);
    void (*init)(struct net_device *, struct vcap_admin *, u32, u32);
    void (*update)(struct net_device *, struct vcap_admin *, enum vcap_command, enum vcap_selection, u32);
    void (*move)(struct net_device *, struct vcap_admin *, u32, int, int);
    int (*port_info)(struct net_device *, struct vcap_admin *, struct vcap_output_print *);
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
<b>Field removed. </b>
<code>int (*enable)(struct net_device *, struct vcap_admin *, bool)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

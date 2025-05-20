# Struct: <code>cec_adap_ops</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
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
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
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
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cec_adap_ops {
    int (*adap_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_all_enable)(struct cec_adapter *, bool);
    int (*adap_monitor_pin_enable)(struct cec_adapter *, bool);
    int (*adap_log_addr)(struct cec_adapter *, u8);
    int (*adap_transmit)(struct cec_adapter *, u8, u32, struct cec_msg *);
    void (*adap_status)(struct cec_adapter *, struct seq_file *);
    void (*adap_free)(struct cec_adapter *);
    int (*error_inj_show)(struct cec_adapter *, struct seq_file *);
    bool (*error_inj_parse_line)(struct cec_adapter *, char *);
    int (*received)(struct cec_adapter *, struct cec_msg *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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

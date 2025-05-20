# Struct: <code>fc_host_attrs</code>

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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fc_host_attrs {
    u64 node_name;
    u64 port_name;
    u64 permanent_port_name;
    u32 supported_classes;
    u8 supported_fc4s[32];
    u32 supported_speeds;
    u32 maxframe_size;
    u16 max_npiv_vports;
    char serial_number[80];
    char manufacturer[80];
    char model[256];
    char model_description[256];
    char hardware_version[64];
    char driver_version[64];
    char firmware_version[64];
    char optionrom_version[64];
    u32 port_id;
    enum fc_port_type port_type;
    enum fc_port_state port_state;
    u8 active_fc4s[32];
    u32 speed;
    u64 fabric_name;
    char symbolic_name[256];
    char system_hostname[256];
    u32 dev_loss_tmo;
    enum fc_tgtid_binding_type tgtid_bind_type;
    struct list_head rports;
    struct list_head rport_bindings;
    struct list_head vports;
    u32 next_rport_number;
    u32 next_target_id;
    u32 next_vport_number;
    u16 npiv_vports_inuse;
    char work_q_name[20];
    struct workqueue_struct *work_q;
    char devloss_work_q_name[20];
    struct workqueue_struct *devloss_work_q;
    struct request_queue *rqst_q;
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Flavor</b>
<ul>
</ul>

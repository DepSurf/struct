# Struct: <code>fc_function_template</code>

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
struct fc_function_template {
    void (*get_rport_dev_loss_tmo)(struct fc_rport *);
    void (*set_rport_dev_loss_tmo)(struct fc_rport *, u32);
    void (*get_starget_node_name)(struct scsi_target *);
    void (*get_starget_port_name)(struct scsi_target *);
    void (*get_starget_port_id)(struct scsi_target *);
    void (*get_host_port_id)(struct Scsi_Host *);
    void (*get_host_port_type)(struct Scsi_Host *);
    void (*get_host_port_state)(struct Scsi_Host *);
    void (*get_host_active_fc4s)(struct Scsi_Host *);
    void (*get_host_speed)(struct Scsi_Host *);
    void (*get_host_fabric_name)(struct Scsi_Host *);
    void (*get_host_symbolic_name)(struct Scsi_Host *);
    void (*set_host_system_hostname)(struct Scsi_Host *);
    struct fc_host_statistics * (*get_fc_host_stats)(struct Scsi_Host *);
    void (*reset_fc_host_stats)(struct Scsi_Host *);
    int (*issue_fc_host_lip)(struct Scsi_Host *);
    void (*dev_loss_tmo_callbk)(struct fc_rport *);
    void (*terminate_rport_io)(struct fc_rport *);
    void (*set_vport_symbolic_name)(struct fc_vport *);
    int (*vport_create)(struct fc_vport *, bool);
    int (*vport_disable)(struct fc_vport *, bool);
    int (*vport_delete)(struct fc_vport *);
    int (*bsg_request)(struct bsg_job *);
    int (*bsg_timeout)(struct bsg_job *);
    u32 dd_fcrport_size;
    u32 dd_fcvport_size;
    u32 dd_bsg_size;
    long unsigned int show_rport_maxframe_size;
    long unsigned int show_rport_supported_classes;
    long unsigned int show_rport_dev_loss_tmo;
    long unsigned int show_starget_node_name;
    long unsigned int show_starget_port_name;
    long unsigned int show_starget_port_id;
    long unsigned int show_host_node_name;
    long unsigned int show_host_port_name;
    long unsigned int show_host_permanent_port_name;
    long unsigned int show_host_supported_classes;
    long unsigned int show_host_supported_fc4s;
    long unsigned int show_host_supported_speeds;
    long unsigned int show_host_maxframe_size;
    long unsigned int show_host_serial_number;
    long unsigned int show_host_manufacturer;
    long unsigned int show_host_model;
    long unsigned int show_host_model_description;
    long unsigned int show_host_hardware_version;
    long unsigned int show_host_driver_version;
    long unsigned int show_host_firmware_version;
    long unsigned int show_host_optionrom_version;
    long unsigned int show_host_port_id;
    long unsigned int show_host_port_type;
    long unsigned int show_host_port_state;
    long unsigned int show_host_active_fc4s;
    long unsigned int show_host_speed;
    long unsigned int show_host_fabric_name;
    long unsigned int show_host_symbolic_name;
    long unsigned int show_host_system_hostname;
    long unsigned int disable_target_scan;
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

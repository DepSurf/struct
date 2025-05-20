# Struct: <code>nvme_command</code>

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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct nvme_command {
    struct nvme_common_command common;
    struct nvme_rw_command rw;
    struct nvme_identify identify;
    struct nvme_features features;
    struct nvme_create_cq create_cq;
    struct nvme_create_sq create_sq;
    struct nvme_delete_queue delete_queue;
    struct nvme_download_firmware dlfw;
    struct nvme_format_cmd format;
    struct nvme_dsm_cmd dsm;
    struct nvme_write_zeroes_cmd write_zeroes;
    struct nvme_abort_cmd abort;
    struct nvme_get_log_page_command get_log_page;
    struct nvmf_common_command fabrics;
    struct nvmf_connect_command connect;
    struct nvmf_property_set_command prop_set;
    struct nvmf_property_get_command prop_get;
    struct nvme_dbbuf dbbuf;
    struct nvme_directive_cmd directive;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvme_command {
    struct nvme_common_command common;
    struct nvme_rw_command rw;
    struct nvme_identify identify;
    struct nvme_features features;
    struct nvme_create_cq create_cq;
    struct nvme_create_sq create_sq;
    struct nvme_delete_queue delete_queue;
    struct nvme_download_firmware dlfw;
    struct nvme_format_cmd format;
    struct nvme_dsm_cmd dsm;
    struct nvme_write_zeroes_cmd write_zeroes;
    struct nvme_abort_cmd abort;
    struct nvme_get_log_page_command get_log_page;
    struct nvmf_common_command fabrics;
    struct nvmf_connect_command connect;
    struct nvmf_property_set_command prop_set;
    struct nvmf_property_get_command prop_get;
    struct nvme_dbbuf dbbuf;
    struct nvme_directive_cmd directive;
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

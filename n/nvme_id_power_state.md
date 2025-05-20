# Struct: <code>nvme_id_power_state</code>

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
struct nvme_id_power_state {
    __le16 max_power;
    __u8 rsvd2;
    __u8 flags;
    __le32 entry_lat;
    __le32 exit_lat;
    __u8 read_tput;
    __u8 read_lat;
    __u8 write_tput;
    __u8 write_lat;
    __le16 idle_power;
    __u8 idle_scale;
    __u8 rsvd19;
    __le16 active_power;
    __u8 active_work_scale;
    __u8 rsvd23[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvme_id_power_state {
    __le16 max_power;
    __u8 rsvd2;
    __u8 flags;
    __le32 entry_lat;
    __le32 exit_lat;
    __u8 read_tput;
    __u8 read_lat;
    __u8 write_tput;
    __u8 write_lat;
    __le16 idle_power;
    __u8 idle_scale;
    __u8 rsvd19;
    __le16 active_power;
    __u8 active_work_scale;
    __u8 rsvd23[9];
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

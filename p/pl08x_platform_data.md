# Struct: <code>pl08x_platform_data</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct pl08x_platform_data {
    struct pl08x_channel_data *slave_channels;
    unsigned int num_slave_channels;
    enum pl08x_burst_size memcpy_burst_size;
    enum pl08x_bus_width memcpy_bus_width;
    bool memcpy_prot_buff;
    bool memcpy_prot_cache;
    int (*get_xfer_signal)(const struct pl08x_channel_data *);
    void (*put_xfer_signal)(const struct pl08x_channel_data *, int);
    u8 lli_buses;
    u8 mem_buses;
    const struct dma_slave_map *slave_map;
    int slave_map_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pl08x_platform_data {
    struct pl08x_channel_data *slave_channels;
    unsigned int num_slave_channels;
    enum pl08x_burst_size memcpy_burst_size;
    enum pl08x_bus_width memcpy_bus_width;
    bool memcpy_prot_buff;
    bool memcpy_prot_cache;
    int (*get_xfer_signal)(const struct pl08x_channel_data *);
    void (*put_xfer_signal)(const struct pl08x_channel_data *, int);
    u8 lli_buses;
    u8 mem_buses;
    const struct dma_slave_map *slave_map;
    int slave_map_len;
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

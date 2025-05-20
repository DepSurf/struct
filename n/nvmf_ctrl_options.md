# Struct: <code>nvmf_ctrl_options</code>

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
struct nvmf_ctrl_options {
    unsigned int mask;
    char *transport;
    char *subsysnqn;
    char *traddr;
    char *trsvcid;
    char *host_traddr;
    size_t queue_size;
    unsigned int nr_io_queues;
    unsigned int reconnect_delay;
    bool discovery_nqn;
    bool duplicate_connect;
    unsigned int kato;
    struct nvmf_host *host;
    int max_reconnects;
    bool disable_sqflow;
    bool hdr_digest;
    bool data_digest;
    unsigned int nr_write_queues;
    unsigned int nr_poll_queues;
    int tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvmf_ctrl_options {
    unsigned int mask;
    char *transport;
    char *subsysnqn;
    char *traddr;
    char *trsvcid;
    char *host_traddr;
    size_t queue_size;
    unsigned int nr_io_queues;
    unsigned int reconnect_delay;
    bool discovery_nqn;
    bool duplicate_connect;
    unsigned int kato;
    struct nvmf_host *host;
    int max_reconnects;
    bool disable_sqflow;
    bool hdr_digest;
    bool data_digest;
    unsigned int nr_write_queues;
    unsigned int nr_poll_queues;
    int tos;
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

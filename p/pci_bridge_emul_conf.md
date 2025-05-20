# Struct: <code>pci_bridge_emul_conf</code>

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
struct pci_bridge_emul_conf {
    u16 vendor;
    u16 device;
    u16 command;
    u16 status;
    u32 class_revision;
    u8 cache_line_size;
    u8 latency_timer;
    u8 header_type;
    u8 bist;
    u32 bar[2];
    u8 primary_bus;
    u8 secondary_bus;
    u8 subordinate_bus;
    u8 secondary_latency_timer;
    u8 iobase;
    u8 iolimit;
    u16 secondary_status;
    u16 membase;
    u16 memlimit;
    u16 pref_mem_base;
    u16 pref_mem_limit;
    u32 prefbaseupper;
    u32 preflimitupper;
    u16 iobaseupper;
    u16 iolimitupper;
    u8 capabilities_pointer;
    u8 reserve[3];
    u32 romaddr;
    u8 intline;
    u8 intpin;
    u16 bridgectrl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_bridge_emul_conf {
    u16 vendor;
    u16 device;
    u16 command;
    u16 status;
    u32 class_revision;
    u8 cache_line_size;
    u8 latency_timer;
    u8 header_type;
    u8 bist;
    u32 bar[2];
    u8 primary_bus;
    u8 secondary_bus;
    u8 subordinate_bus;
    u8 secondary_latency_timer;
    u8 iobase;
    u8 iolimit;
    u16 secondary_status;
    u16 membase;
    u16 memlimit;
    u16 pref_mem_base;
    u16 pref_mem_limit;
    u32 prefbaseupper;
    u32 preflimitupper;
    u16 iobaseupper;
    u16 iolimitupper;
    u8 capabilities_pointer;
    u8 reserve[3];
    u32 romaddr;
    u8 intline;
    u8 intpin;
    u16 bridgectrl;
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

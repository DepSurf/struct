# Struct: <code>pci_bridge_emul_pcie_conf</code>

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
struct pci_bridge_emul_pcie_conf {
    u8 cap_id;
    u8 next;
    u16 cap;
    u32 devcap;
    u16 devctl;
    u16 devsta;
    u32 lnkcap;
    u16 lnkctl;
    u16 lnksta;
    u32 slotcap;
    u16 slotctl;
    u16 slotsta;
    u16 rootctl;
    u16 rsvd;
    u32 rootsta;
    u32 devcap2;
    u16 devctl2;
    u16 devsta2;
    u32 lnkcap2;
    u16 lnkctl2;
    u16 lnksta2;
    u32 slotcap2;
    u16 slotctl2;
    u16 slotsta2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_bridge_emul_pcie_conf {
    u8 cap_id;
    u8 next;
    u16 cap;
    u32 devcap;
    u16 devctl;
    u16 devsta;
    u32 lnkcap;
    u16 lnkctl;
    u16 lnksta;
    u32 slotcap;
    u16 slotctl;
    u16 slotsta;
    u16 rootctl;
    u16 rsvd;
    u32 rootsta;
    u32 devcap2;
    u16 devctl2;
    u16 devsta2;
    u32 lnkcap2;
    u16 lnkctl2;
    u16 lnksta2;
    u32 slotcap2;
    u16 slotctl2;
    u16 slotsta2;
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

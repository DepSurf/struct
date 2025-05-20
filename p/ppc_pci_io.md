# Struct: <code>ppc_pci_io</code>

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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ppc_pci_io {
    u8 (*readb)(volatile const void *);
    u16 (*readw)(volatile const void *);
    u32 (*readl)(volatile const void *);
    u16 (*readw_be)(volatile const void *);
    u32 (*readl_be)(volatile const void *);
    void (*writeb)(u8, volatile void *);
    void (*writew)(u16, volatile void *);
    void (*writel)(u32, volatile void *);
    void (*writew_be)(u16, volatile void *);
    void (*writel_be)(u32, volatile void *);
    u64 (*readq)(volatile const void *);
    u64 (*readq_be)(volatile const void *);
    void (*writeq)(u64, volatile void *);
    void (*writeq_be)(u64, volatile void *);
    u8 (*inb)(long unsigned int);
    u16 (*inw)(long unsigned int);
    u32 (*inl)(long unsigned int);
    void (*outb)(u8, long unsigned int);
    void (*outw)(u16, long unsigned int);
    void (*outl)(u32, long unsigned int);
    void (*readsb)(volatile const void *, void *, long unsigned int);
    void (*readsw)(volatile const void *, void *, long unsigned int);
    void (*readsl)(volatile const void *, void *, long unsigned int);
    void (*writesb)(volatile void *, const void *, long unsigned int);
    void (*writesw)(volatile void *, const void *, long unsigned int);
    void (*writesl)(volatile void *, const void *, long unsigned int);
    void (*insb)(long unsigned int, void *, long unsigned int);
    void (*insw)(long unsigned int, void *, long unsigned int);
    void (*insl)(long unsigned int, void *, long unsigned int);
    void (*outsb)(long unsigned int, const void *, long unsigned int);
    void (*outsw)(long unsigned int, const void *, long unsigned int);
    void (*outsl)(long unsigned int, const void *, long unsigned int);
    void (*memset_io)(volatile void *, int, long unsigned int);
    void (*memcpy_fromio)(void *, volatile const void *, long unsigned int);
    void (*memcpy_toio)(volatile void *, const void *, long unsigned int);
};
```
</details>
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

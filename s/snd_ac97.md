# Struct: <code>snd_ac97</code>

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
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct snd_ac97 {
    const struct snd_ac97_build_ops *build_ops;
    void *private_data;
    void (*private_free)(struct snd_ac97 *);
    struct snd_ac97_bus *bus;
    struct pci_dev *pci;
    struct snd_info_entry *proc;
    struct snd_info_entry *proc_regs;
    short unsigned int subsystem_vendor;
    short unsigned int subsystem_device;
    struct mutex reg_mutex;
    struct mutex page_mutex;
    short unsigned int num;
    short unsigned int addr;
    unsigned int id;
    short unsigned int caps;
    short unsigned int ext_id;
    short unsigned int ext_mid;
    const struct snd_ac97_res_table *res_table;
    unsigned int scaps;
    unsigned int flags;
    unsigned int rates[6];
    unsigned int spdif_status;
    short unsigned int regs[128];
    long unsigned int reg_accessed[4];
    union (anon) spec;
    unsigned char indep_surround;
    unsigned char channel_mode;
    unsigned int power_up;
    struct delayed_work power_work;
    struct device dev;
    struct snd_ac97_gpio_priv *gpio_priv;
    struct snd_pcm_chmap * chmaps[2];
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

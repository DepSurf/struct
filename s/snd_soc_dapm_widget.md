# Struct: <code>snd_soc_dapm_widget</code>

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
struct snd_soc_dapm_widget {
    enum snd_soc_dapm_type id;
    const char *name;
    const char *sname;
    struct list_head list;
    struct snd_soc_dapm_context *dapm;
    void *priv;
    struct regulator *regulator;
    struct pinctrl *pinctrl;
    int reg;
    unsigned char shift;
    unsigned int mask;
    unsigned int on_val;
    unsigned int off_val;
    unsigned char power;
    unsigned char active;
    unsigned char connected;
    unsigned char new;
    unsigned char force;
    unsigned char ignore_suspend;
    unsigned char new_power;
    unsigned char power_checked;
    unsigned char is_supply;
    unsigned char is_ep;
    int subseq;
    int (*power_check)(struct snd_soc_dapm_widget *);
    short unsigned int event_flags;
    int (*event)(struct snd_soc_dapm_widget *, struct snd_kcontrol *, int);
    int num_kcontrols;
    const struct snd_kcontrol_new *kcontrol_news;
    struct snd_kcontrol **kcontrols;
    struct snd_soc_dobj dobj;
    struct list_head edges[2];
    struct list_head work_list;
    struct list_head power_list;
    struct list_head dirty;
    int endpoints[2];
    struct clk *clk;
    int channel;
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

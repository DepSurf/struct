# Struct: <code>snd_soc_component_driver</code>

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
struct snd_soc_component_driver {
    const char *name;
    const struct snd_kcontrol_new *controls;
    unsigned int num_controls;
    const struct snd_soc_dapm_widget *dapm_widgets;
    unsigned int num_dapm_widgets;
    const struct snd_soc_dapm_route *dapm_routes;
    unsigned int num_dapm_routes;
    int (*probe)(struct snd_soc_component *);
    void (*remove)(struct snd_soc_component *);
    int (*suspend)(struct snd_soc_component *);
    int (*resume)(struct snd_soc_component *);
    unsigned int (*read)(struct snd_soc_component *, unsigned int);
    int (*write)(struct snd_soc_component *, unsigned int, unsigned int);
    int (*pcm_new)(struct snd_soc_pcm_runtime *);
    void (*pcm_free)(struct snd_pcm *);
    int (*set_sysclk)(struct snd_soc_component *, int, int, unsigned int, int);
    int (*set_pll)(struct snd_soc_component *, int, int, unsigned int, unsigned int);
    int (*set_jack)(struct snd_soc_component *, struct snd_soc_jack *, void *);
    int (*of_xlate_dai_name)(struct snd_soc_component *, struct of_phandle_args *, const char **);
    int (*of_xlate_dai_id)(struct snd_soc_component *, struct device_node *);
    void (*seq_notifier)(struct snd_soc_component *, enum snd_soc_dapm_type, int);
    int (*stream_event)(struct snd_soc_component *, int);
    int (*set_bias_level)(struct snd_soc_component *, enum snd_soc_bias_level);
    const struct snd_pcm_ops *ops;
    const struct snd_compr_ops *compr_ops;
    int probe_order;
    int remove_order;
    unsigned int module_get_upon_open;
    unsigned int idle_bias_on;
    unsigned int suspend_bias_off;
    unsigned int use_pmdown_time;
    unsigned int endianness;
    unsigned int non_legacy_dai_naming;
    const char *ignore_machine;
    const char *topology_name_prefix;
    int (*be_hw_params_fixup)(struct snd_soc_pcm_runtime *, struct snd_pcm_hw_params *);
    bool use_dai_pcm_id;
    int be_pcm_base;
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

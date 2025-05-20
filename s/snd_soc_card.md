# Struct: <code>snd_soc_card</code>

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
struct snd_soc_card {
    const char *name;
    const char *long_name;
    const char *driver_name;
    const char *components;
    char dmi_longname[80];
    char topology_shortname[32];
    struct device *dev;
    struct snd_card *snd_card;
    struct module *owner;
    struct mutex mutex;
    struct mutex dapm_mutex;
    struct mutex pcm_mutex;
    enum snd_soc_pcm_subclass pcm_subclass;
    spinlock_t dpcm_lock;
    bool instantiated;
    bool topology_shortname_created;
    int (*probe)(struct snd_soc_card *);
    int (*late_probe)(struct snd_soc_card *);
    int (*remove)(struct snd_soc_card *);
    int (*suspend_pre)(struct snd_soc_card *);
    int (*suspend_post)(struct snd_soc_card *);
    int (*resume_pre)(struct snd_soc_card *);
    int (*resume_post)(struct snd_soc_card *);
    int (*set_bias_level)(struct snd_soc_card *, struct snd_soc_dapm_context *, enum snd_soc_bias_level);
    int (*set_bias_level_post)(struct snd_soc_card *, struct snd_soc_dapm_context *, enum snd_soc_bias_level);
    int (*add_dai_link)(struct snd_soc_card *, struct snd_soc_dai_link *);
    void (*remove_dai_link)(struct snd_soc_card *, struct snd_soc_dai_link *);
    long int pmdown_time;
    struct snd_soc_dai_link *dai_link;
    int num_links;
    struct list_head dai_link_list;
    struct list_head rtd_list;
    int num_rtd;
    struct snd_soc_codec_conf *codec_conf;
    int num_configs;
    struct snd_soc_aux_dev *aux_dev;
    int num_aux_devs;
    struct list_head aux_comp_list;
    const struct snd_kcontrol_new *controls;
    int num_controls;
    const struct snd_soc_dapm_widget *dapm_widgets;
    int num_dapm_widgets;
    const struct snd_soc_dapm_route *dapm_routes;
    int num_dapm_routes;
    const struct snd_soc_dapm_widget *of_dapm_widgets;
    int num_of_dapm_widgets;
    const struct snd_soc_dapm_route *of_dapm_routes;
    int num_of_dapm_routes;
    bool fully_routed;
    struct list_head component_dev_list;
    struct list_head list;
    struct list_head widgets;
    struct list_head paths;
    struct list_head dapm_list;
    struct list_head dapm_dirty;
    struct list_head dobj_list;
    struct snd_soc_dapm_context dapm;
    struct snd_soc_dapm_stats dapm_stats;
    struct snd_soc_dapm_update *update;
    struct dentry *debugfs_card_root;
    struct work_struct deferred_resume_work;
    u32 pop_time;
    void *drvdata;
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

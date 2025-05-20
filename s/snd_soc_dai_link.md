# Struct: <code>snd_soc_dai_link</code>

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
struct snd_soc_dai_link {
    const char *name;
    const char *stream_name;
    struct snd_soc_dai_link_component *cpus;
    unsigned int num_cpus;
    struct snd_soc_dai_link_component *codecs;
    unsigned int num_codecs;
    struct snd_soc_dai_link_component *platforms;
    unsigned int num_platforms;
    int id;
    const struct snd_soc_pcm_stream *params;
    unsigned int num_params;
    unsigned int dai_fmt;
    enum snd_soc_dpcm_trigger trigger[2];
    int (*init)(struct snd_soc_pcm_runtime *);
    int (*be_hw_params_fixup)(struct snd_soc_pcm_runtime *, struct snd_pcm_hw_params *);
    const struct snd_soc_ops *ops;
    const struct snd_soc_compr_ops *compr_ops;
    bool nonatomic;
    unsigned int playback_only;
    unsigned int capture_only;
    unsigned int ignore_suspend;
    unsigned int symmetric_rates;
    unsigned int symmetric_channels;
    unsigned int symmetric_samplebits;
    unsigned int no_pcm;
    unsigned int dynamic;
    unsigned int dpcm_capture;
    unsigned int dpcm_playback;
    unsigned int dpcm_merged_format;
    unsigned int dpcm_merged_chan;
    unsigned int dpcm_merged_rate;
    unsigned int ignore_pmdown_time;
    unsigned int ignore;
    struct list_head list;
    struct snd_soc_dobj dobj;
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

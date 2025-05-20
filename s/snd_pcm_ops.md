# Struct: <code>snd_pcm_ops</code>

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
struct snd_pcm_ops {
    int (*open)(struct snd_pcm_substream *);
    int (*close)(struct snd_pcm_substream *);
    int (*ioctl)(struct snd_pcm_substream *, unsigned int, void *);
    int (*hw_params)(struct snd_pcm_substream *, struct snd_pcm_hw_params *);
    int (*hw_free)(struct snd_pcm_substream *);
    int (*prepare)(struct snd_pcm_substream *);
    int (*trigger)(struct snd_pcm_substream *, int);
    snd_pcm_uframes_t (*pointer)(struct snd_pcm_substream *);
    int (*get_time_info)(struct snd_pcm_substream *, struct timespec *, struct timespec *, struct snd_pcm_audio_tstamp_config *, struct snd_pcm_audio_tstamp_report *);
    int (*fill_silence)(struct snd_pcm_substream *, int, long unsigned int, long unsigned int);
    int (*copy_user)(struct snd_pcm_substream *, int, long unsigned int, void *, long unsigned int);
    int (*copy_kernel)(struct snd_pcm_substream *, int, long unsigned int, void *, long unsigned int);
    struct page * (*page)(struct snd_pcm_substream *, long unsigned int);
    int (*mmap)(struct snd_pcm_substream *, struct vm_area_struct *);
    int (*ack)(struct snd_pcm_substream *);
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

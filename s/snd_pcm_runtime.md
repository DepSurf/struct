# Struct: <code>snd_pcm_runtime</code>

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
struct snd_pcm_runtime {
    struct snd_pcm_substream *trigger_master;
    struct timespec trigger_tstamp;
    bool trigger_tstamp_latched;
    int overrange;
    snd_pcm_uframes_t avail_max;
    snd_pcm_uframes_t hw_ptr_base;
    snd_pcm_uframes_t hw_ptr_interrupt;
    long unsigned int hw_ptr_jiffies;
    long unsigned int hw_ptr_buffer_jiffies;
    snd_pcm_sframes_t delay;
    u64 hw_ptr_wrap;
    snd_pcm_access_t access;
    snd_pcm_format_t format;
    snd_pcm_subformat_t subformat;
    unsigned int rate;
    unsigned int channels;
    snd_pcm_uframes_t period_size;
    unsigned int periods;
    snd_pcm_uframes_t buffer_size;
    snd_pcm_uframes_t min_align;
    size_t byte_align;
    unsigned int frame_bits;
    unsigned int sample_bits;
    unsigned int info;
    unsigned int rate_num;
    unsigned int rate_den;
    unsigned int no_period_wakeup;
    int tstamp_mode;
    unsigned int period_step;
    snd_pcm_uframes_t start_threshold;
    snd_pcm_uframes_t stop_threshold;
    snd_pcm_uframes_t silence_threshold;
    snd_pcm_uframes_t silence_size;
    snd_pcm_uframes_t boundary;
    snd_pcm_uframes_t silence_start;
    snd_pcm_uframes_t silence_filled;
    union snd_pcm_sync_id sync;
    struct snd_pcm_mmap_status *status;
    struct snd_pcm_mmap_control *control;
    snd_pcm_uframes_t twake;
    wait_queue_head_t sleep;
    wait_queue_head_t tsleep;
    struct fasync_struct *fasync;
    void *private_data;
    void (*private_free)(struct snd_pcm_runtime *);
    struct snd_pcm_hardware hw;
    struct snd_pcm_hw_constraints hw_constraints;
    unsigned int timer_resolution;
    int tstamp_type;
    unsigned char *dma_area;
    dma_addr_t dma_addr;
    size_t dma_bytes;
    struct snd_dma_buffer *dma_buffer_p;
    struct snd_pcm_audio_tstamp_config audio_tstamp_config;
    struct snd_pcm_audio_tstamp_report audio_tstamp_report;
    struct timespec driver_tstamp;
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

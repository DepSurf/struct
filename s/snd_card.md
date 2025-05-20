# Struct: <code>snd_card</code>

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
struct snd_card {
    int number;
    char id[16];
    char driver[16];
    char shortname[32];
    char longname[80];
    char irq_descr[32];
    char mixername[80];
    char components[128];
    struct module *module;
    void *private_data;
    void (*private_free)(struct snd_card *);
    struct list_head devices;
    struct device ctl_dev;
    unsigned int last_numid;
    struct rw_semaphore controls_rwsem;
    rwlock_t ctl_files_rwlock;
    int controls_count;
    int user_ctl_count;
    struct list_head controls;
    struct list_head ctl_files;
    struct snd_info_entry *proc_root;
    struct proc_dir_entry *proc_root_link;
    struct list_head files_list;
    struct snd_shutdown_f_ops *s_f_ops;
    spinlock_t files_lock;
    int shutdown;
    struct completion *release_completion;
    struct device *dev;
    struct device card_dev;
    const struct attribute_group * dev_groups[4];
    bool registered;
    wait_queue_head_t remove_sleep;
    unsigned int power_state;
    wait_queue_head_t power_sleep;
    struct snd_mixer_oss *mixer_oss;
    int mixer_oss_change_count;
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

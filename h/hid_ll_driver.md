# Struct: <code>hid_ll_driver</code>

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
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hid_ll_driver {
    int (*start)(struct hid_device *);
    void (*stop)(struct hid_device *);
    int (*open)(struct hid_device *);
    void (*close)(struct hid_device *);
    int (*power)(struct hid_device *, int);
    int (*parse)(struct hid_device *);
    void (*request)(struct hid_device *, struct hid_report *, int);
    int (*wait)(struct hid_device *);
    int (*raw_request)(struct hid_device *, unsigned char, __u8 *, size_t, unsigned char, int);
    int (*output_report)(struct hid_device *, __u8 *, size_t);
    int (*idle)(struct hid_device *, int, int, int);
    bool (*may_wakeup)(struct hid_device *);
    unsigned int max_buffer_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hid_ll_driver {
    int (*start)(struct hid_device *);
    void (*stop)(struct hid_device *);
    int (*open)(struct hid_device *);
    void (*close)(struct hid_device *);
    int (*power)(struct hid_device *, int);
    int (*parse)(struct hid_device *);
    void (*request)(struct hid_device *, struct hid_report *, int);
    int (*wait)(struct hid_device *);
    int (*raw_request)(struct hid_device *, unsigned char, __u8 *, size_t, unsigned char, int);
    int (*output_report)(struct hid_device *, __u8 *, size_t);
    int (*idle)(struct hid_device *, int, int, int);
    bool (*may_wakeup)(struct hid_device *);
    unsigned int max_buffer_size;
};
```
</details>
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
<b>Regular</b>
<ul>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

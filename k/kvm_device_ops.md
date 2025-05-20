# Struct: <code>kvm_device_ops</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct kvm_device_ops {
    const char *name;
    int (*create)(struct kvm_device *, u32);
    void (*init)(struct kvm_device *);
    void (*destroy)(struct kvm_device *);
    void (*release)(struct kvm_device *);
    int (*set_attr)(struct kvm_device *, struct kvm_device_attr *);
    int (*get_attr)(struct kvm_device *, struct kvm_device_attr *);
    int (*has_attr)(struct kvm_device *, struct kvm_device_attr *);
    long int (*ioctl)(struct kvm_device *, unsigned int, long unsigned int);
    int (*mmap)(struct kvm_device *, struct vm_area_struct *);
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kvm_device_ops {
    const char *name;
    int (*create)(struct kvm_device *, u32);
    void (*init)(struct kvm_device *);
    void (*destroy)(struct kvm_device *);
    void (*release)(struct kvm_device *);
    int (*set_attr)(struct kvm_device *, struct kvm_device_attr *);
    int (*get_attr)(struct kvm_device *, struct kvm_device_attr *);
    int (*has_attr)(struct kvm_device *, struct kvm_device_attr *);
    long int (*ioctl)(struct kvm_device *, unsigned int, long unsigned int);
    int (*mmap)(struct kvm_device *, struct vm_area_struct *);
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

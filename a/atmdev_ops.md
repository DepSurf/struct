# Struct: <code>atmdev_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct atmdev_ops {
    void (*dev_close)(struct atm_dev *);
    int (*open)(struct atm_vcc *);
    void (*close)(struct atm_vcc *);
    int (*ioctl)(struct atm_dev *, unsigned int, void *);
    int (*compat_ioctl)(struct atm_dev *, unsigned int, void *);
    int (*getsockopt)(struct atm_vcc *, int, int, void *, int);
    int (*setsockopt)(struct atm_vcc *, int, int, void *, unsigned int);
    int (*send)(struct atm_vcc *, struct sk_buff *);
    int (*send_oam)(struct atm_vcc *, void *, int);
    void (*phy_put)(struct atm_dev *, unsigned char, long unsigned int);
    unsigned char (*phy_get)(struct atm_dev *, long unsigned int);
    int (*change_qos)(struct atm_vcc *, struct atm_qos *, int);
    int (*proc_read)(struct atm_dev *, loff_t *, char *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct atmdev_ops {
    void (*dev_close)(struct atm_dev *);
    int (*open)(struct atm_vcc *);
    void (*close)(struct atm_vcc *);
    int (*ioctl)(struct atm_dev *, unsigned int, void *);
    int (*compat_ioctl)(struct atm_dev *, unsigned int, void *);
    int (*getsockopt)(struct atm_vcc *, int, int, void *, int);
    int (*setsockopt)(struct atm_vcc *, int, int, void *, unsigned int);
    int (*send)(struct atm_vcc *, struct sk_buff *);
    int (*send_oam)(struct atm_vcc *, void *, int);
    void (*phy_put)(struct atm_dev *, unsigned char, long unsigned int);
    unsigned char (*phy_get)(struct atm_dev *, long unsigned int);
    int (*change_qos)(struct atm_vcc *, struct atm_qos *, int);
    int (*proc_read)(struct atm_dev *, loff_t *, char *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct atmdev_ops {
    void (*dev_close)(struct atm_dev *);
    int (*open)(struct atm_vcc *);
    void (*close)(struct atm_vcc *);
    int (*ioctl)(struct atm_dev *, unsigned int, void *);
    int (*compat_ioctl)(struct atm_dev *, unsigned int, void *);
    int (*getsockopt)(struct atm_vcc *, int, int, void *, int);
    int (*setsockopt)(struct atm_vcc *, int, int, void *, unsigned int);
    int (*send)(struct atm_vcc *, struct sk_buff *);
    int (*send_oam)(struct atm_vcc *, void *, int);
    void (*phy_put)(struct atm_dev *, unsigned char, long unsigned int);
    unsigned char (*phy_get)(struct atm_dev *, long unsigned int);
    int (*change_qos)(struct atm_vcc *, struct atm_qos *, int);
    int (*proc_read)(struct atm_dev *, loff_t *, char *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct atmdev_ops {
    void (*dev_close)(struct atm_dev *);
    int (*open)(struct atm_vcc *);
    void (*close)(struct atm_vcc *);
    int (*ioctl)(struct atm_dev *, unsigned int, void *);
    int (*compat_ioctl)(struct atm_dev *, unsigned int, void *);
    int (*getsockopt)(struct atm_vcc *, int, int, void *, int);
    int (*setsockopt)(struct atm_vcc *, int, int, void *, unsigned int);
    int (*send)(struct atm_vcc *, struct sk_buff *);
    int (*send_oam)(struct atm_vcc *, void *, int);
    void (*phy_put)(struct atm_dev *, unsigned char, long unsigned int);
    unsigned char (*phy_get)(struct atm_dev *, long unsigned int);
    int (*change_qos)(struct atm_vcc *, struct atm_qos *, int);
    int (*proc_read)(struct atm_dev *, loff_t *, char *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct atmdev_ops {
    void (*dev_close)(struct atm_dev *);
    int (*open)(struct atm_vcc *);
    void (*close)(struct atm_vcc *);
    int (*ioctl)(struct atm_dev *, unsigned int, void *);
    int (*compat_ioctl)(struct atm_dev *, unsigned int, void *);
    int (*getsockopt)(struct atm_vcc *, int, int, void *, int);
    int (*setsockopt)(struct atm_vcc *, int, int, void *, unsigned int);
    int (*send)(struct atm_vcc *, struct sk_buff *);
    int (*send_oam)(struct atm_vcc *, void *, int);
    void (*phy_put)(struct atm_dev *, unsigned char, long unsigned int);
    unsigned char (*phy_get)(struct atm_dev *, long unsigned int);
    int (*change_qos)(struct atm_vcc *, struct atm_qos *, int);
    int (*proc_read)(struct atm_dev *, loff_t *, char *);
    struct module *owner;
};
```
</details>
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
</ul>

# Struct: <code>compat_rtentry</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_rtentry {
    u32 rt_pad1;
    struct sockaddr rt_dst;
    struct sockaddr rt_gateway;
    struct sockaddr rt_genmask;
    short unsigned int rt_flags;
    short int rt_pad2;
    u32 rt_pad3;
    unsigned char rt_tos;
    unsigned char rt_class;
    short int rt_pad4;
    short int rt_metric;
    compat_uptr_t rt_dev;
    u32 rt_mtu;
    u32 rt_window;
    short unsigned int rt_irtt;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>

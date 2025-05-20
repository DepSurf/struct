# Struct: <code>clcd_board</code>

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
struct clcd_board {
    const char *name;
    u32 caps;
    int (*check)(struct clcd_fb *, struct fb_var_screeninfo *);
    void (*decode)(struct clcd_fb *, struct clcd_regs *);
    void (*disable)(struct clcd_fb *);
    void (*enable)(struct clcd_fb *);
    int (*setup)(struct clcd_fb *);
    int (*mmap)(struct clcd_fb *, struct vm_area_struct *);
    void (*remove)(struct clcd_fb *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct clcd_board {
    const char *name;
    u32 caps;
    int (*check)(struct clcd_fb *, struct fb_var_screeninfo *);
    void (*decode)(struct clcd_fb *, struct clcd_regs *);
    void (*disable)(struct clcd_fb *);
    void (*enable)(struct clcd_fb *);
    int (*setup)(struct clcd_fb *);
    int (*mmap)(struct clcd_fb *, struct vm_area_struct *);
    void (*remove)(struct clcd_fb *);
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

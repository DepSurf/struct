# Struct: <code>rtc_class_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*open)(struct device *);
    void (*release)(struct device *);
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*open)(struct device *);
    void (*release)(struct device *);
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*open)(struct device *);
    void (*release)(struct device *);
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*open)(struct device *);
    void (*release)(struct device *);
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*set_mmss64)(struct device *, time64_t);
    int (*set_mmss)(struct device *, long unsigned int);
    int (*read_callback)(struct device *, int);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
    int (*param_get)(struct device *, struct rtc_param *);
    int (*param_set)(struct device *, struct rtc_param *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
    int (*param_get)(struct device *, struct rtc_param *);
    int (*param_set)(struct device *, struct rtc_param *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
    int (*param_get)(struct device *, struct rtc_param *);
    int (*param_set)(struct device *, struct rtc_param *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
    int (*param_get)(struct device *, struct rtc_param *);
    int (*param_set)(struct device *, struct rtc_param *);
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rtc_class_ops {
    int (*ioctl)(struct device *, unsigned int, long unsigned int);
    int (*read_time)(struct device *, struct rtc_time *);
    int (*set_time)(struct device *, struct rtc_time *);
    int (*read_alarm)(struct device *, struct rtc_wkalrm *);
    int (*set_alarm)(struct device *, struct rtc_wkalrm *);
    int (*proc)(struct device *, struct seq_file *);
    int (*alarm_irq_enable)(struct device *, unsigned int);
    int (*read_offset)(struct device *, long int *);
    int (*set_offset)(struct device *, long int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*read_offset)(struct device *, long int *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_offset)(struct device *, long int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*open)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*release)(struct device *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*set_mmss64)(struct device *, time64_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_mmss)(struct device *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*read_callback)(struct device *, int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*param_get)(struct device *, struct rtc_param *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*param_set)(struct device *, struct rtc_param *)</code>
</li>
</ul>
</details>
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
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

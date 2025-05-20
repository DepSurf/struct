# Struct: <code>ehci_platform_priv</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[3];
    struct reset_control *rst;
    struct phy **phys;
    int num_phys;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[3];
    struct reset_control * rsts[3];
    struct phy **phys;
    int num_phys;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control * rsts[4];
    struct phy **phys;
    int num_phys;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control * rsts[4];
    struct phy **phys;
    int num_phys;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    struct phy **phys;
    int num_phys;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
    bool quirk_poll;
    struct timer_list poll_timer;
    struct delayed_work poll_work;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ehci_platform_priv {
    struct clk * clks[4];
    struct reset_control *rsts;
    bool reset_on_resume;
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
<code>struct reset_control * rsts[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct reset_control *rst</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct clk * clks[3]</code> ➡️ <code>struct clk * clks[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct reset_control * rsts[3]</code> ➡️ <code>struct reset_control * rsts[4]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct reset_control * rsts[4]</code> ➡️ <code>struct reset_control *rsts</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct phy **phys</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_phys</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool quirk_poll</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list poll_timer</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work poll_work</code>
</li>
</ul>
</details>
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
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

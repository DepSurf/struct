# Struct: <code>simplefb_par</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
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
struct simplefb_par {
    u32 palette[16];
    bool clks_enabled;
    unsigned int clk_count;
    struct clk **clks;
    bool regulators_enabled;
    u32 regulator_count;
    struct regulator **regulators;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
    bool clks_enabled;
    unsigned int clk_count;
    struct clk **clks;
    bool regulators_enabled;
    u32 regulator_count;
    struct regulator **regulators;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
    bool regulators_enabled;
    u32 regulator_count;
    struct regulator **regulators;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
    bool clks_enabled;
    unsigned int clk_count;
    struct clk **clks;
    bool regulators_enabled;
    u32 regulator_count;
    struct regulator **regulators;
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
struct simplefb_par {
    u32 palette[16];
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
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct simplefb_par {
    u32 palette[16];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool clks_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int clk_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct clk **clks</code>
</li>
<li>
<b>Field added. </b>
<code>bool regulators_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u32 regulator_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct regulator **regulators</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool clks_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int clk_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct clk **clks</code>
</li>
<li>
<b>Field added. </b>
<code>bool regulators_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u32 regulator_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct regulator **regulators</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool regulators_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u32 regulator_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct regulator **regulators</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool clks_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int clk_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct clk **clks</code>
</li>
<li>
<b>Field added. </b>
<code>bool regulators_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u32 regulator_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct regulator **regulators</code>
</li>
</ul>
</details>
</li>
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

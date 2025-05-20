# Struct: <code>x86_legacy_features</code>

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
struct x86_legacy_features {
    int rtc;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
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
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct x86_legacy_features {
    enum x86_legacy_i8042_state i8042;
    int rtc;
    int warm_reset;
    int no_vga;
    int reserve_bios_regions;
    struct x86_legacy_devices devices;
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum x86_legacy_i8042_state i8042</code>
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
<b>Field added. </b>
<code>int no_vga</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int warm_reset</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

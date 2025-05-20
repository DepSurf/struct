# Struct: <code>em_data_callback</code>

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
struct em_data_callback {
    int (*active_power)(long unsigned int *, long unsigned int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(long unsigned int *, long unsigned int *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(long unsigned int *, long unsigned int *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(long unsigned int *, long unsigned int *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(struct device *, long unsigned int *, long unsigned int *);
    int (*get_cost)(struct device *, long unsigned int, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(struct device *, long unsigned int *, long unsigned int *);
    int (*get_cost)(struct device *, long unsigned int, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(struct device *, long unsigned int *, long unsigned int *);
    int (*get_cost)(struct device *, long unsigned int, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct em_data_callback {
    int (*active_power)(struct device *, long unsigned int *, long unsigned int *);
    int (*get_cost)(struct device *, long unsigned int, long unsigned int *);
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
struct em_data_callback {
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct em_data_callback {
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct em_data_callback {
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct em_data_callback {
};
```
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*active_power)(long unsigned int *, long unsigned int *, int)</code> ➡️ <code>int (*active_power)(long unsigned int *, long unsigned int *, struct device *)</code>
</li>
</ul>
</details>
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
<code>int (*get_cost)(struct device *, long unsigned int, long unsigned int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*active_power)(long unsigned int *, long unsigned int *, struct device *)</code> ➡️ <code>int (*active_power)(struct device *, long unsigned int *, long unsigned int *)</code>
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
</ul>

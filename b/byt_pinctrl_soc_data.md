# Struct: <code>byt_pinctrl_soc_data</code>

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
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct byt_pingroup *groups;
    size_t ngroups;
    const struct byt_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct byt_pingroup *groups;
    size_t ngroups;
    const struct byt_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct byt_pingroup *groups;
    size_t ngroups;
    const struct byt_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct byt_pingroup *groups;
    size_t ngroups;
    const struct byt_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct byt_pingroup *groups;
    size_t ngroups;
    const struct byt_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct byt_pingroup *groups;
    size_t ngroups;
    const struct byt_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct byt_pinctrl_soc_data {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct intel_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct byt_community *communities;
    size_t ncommunities;
};
```
</details>
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
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>const struct byt_pingroup *groups</code> ➡️ <code>const struct intel_pingroup *groups</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct byt_function *functions</code> ➡️ <code>const struct intel_function *functions</code>
</li>
</ul>
</details>
</li>
</ul>

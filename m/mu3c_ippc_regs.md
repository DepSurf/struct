# Struct: <code>mu3c_ippc_regs</code>

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
struct mu3c_ippc_regs {
    __le32 ip_pw_ctr0;
    __le32 ip_pw_ctr1;
    __le32 ip_pw_ctr2;
    __le32 ip_pw_ctr3;
    __le32 ip_pw_sts1;
    __le32 ip_pw_sts2;
    __le32 reserved0[3];
    __le32 ip_xhci_cap;
    __le32 reserved1[2];
    __le64 u3_ctrl_p[4];
    __le64 u2_ctrl_p[5];
    __le32 reserved2;
    __le32 u2_phy_pll;
    __le32 reserved3[33];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mu3c_ippc_regs {
    __le32 ip_pw_ctr0;
    __le32 ip_pw_ctr1;
    __le32 ip_pw_ctr2;
    __le32 ip_pw_ctr3;
    __le32 ip_pw_sts1;
    __le32 ip_pw_sts2;
    __le32 reserved0[3];
    __le32 ip_xhci_cap;
    __le32 reserved1[2];
    __le64 u3_ctrl_p[4];
    __le64 u2_ctrl_p[5];
    __le32 reserved2;
    __le32 u2_phy_pll;
    __le32 reserved3[33];
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

# Struct: <code>uv1_bau_msg_header</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uv1_bau_msg_header {
    unsigned int dest_subnodeid;
    unsigned int base_dest_nasid;
    unsigned int command;
    unsigned int rsvd_1;
    unsigned int rsvd_2;
    unsigned int sequence;
    unsigned int rsvd_3;
    unsigned int replied_to;
    unsigned int msg_type;
    unsigned int canceled;
    unsigned int payload_1a;
    unsigned int payload_1b;
    unsigned int payload_1ca;
    unsigned int payload_1c;
    unsigned int payload_1d;
    unsigned int payload_1e;
    unsigned int rsvd_4;
    unsigned int swack_flag;
    unsigned int rsvd_5;
    unsigned int rsvd_6;
    unsigned int int_both;
    unsigned int fairness;
    unsigned int multilevel;
    unsigned int chaining;
    unsigned int rsvd_7;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uv1_bau_msg_header {
    unsigned int dest_subnodeid;
    unsigned int base_dest_nasid;
    unsigned int command;
    unsigned int rsvd_1;
    unsigned int rsvd_2;
    unsigned int sequence;
    unsigned int rsvd_3;
    unsigned int replied_to;
    unsigned int msg_type;
    unsigned int canceled;
    unsigned int payload_1a;
    unsigned int payload_1b;
    unsigned int payload_1ca;
    unsigned int payload_1c;
    unsigned int payload_1d;
    unsigned int payload_1e;
    unsigned int rsvd_4;
    unsigned int swack_flag;
    unsigned int rsvd_5;
    unsigned int rsvd_6;
    unsigned int int_both;
    unsigned int fairness;
    unsigned int multilevel;
    unsigned int chaining;
    unsigned int rsvd_7;
};
```
</details>
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
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uv1_bau_msg_header {
    unsigned int dest_subnodeid;
    unsigned int base_dest_nasid;
    unsigned int command;
    unsigned int rsvd_1;
    unsigned int rsvd_2;
    unsigned int sequence;
    unsigned int rsvd_3;
    unsigned int replied_to;
    unsigned int msg_type;
    unsigned int canceled;
    unsigned int payload_1a;
    unsigned int payload_1b;
    unsigned int payload_1ca;
    unsigned int payload_1c;
    unsigned int payload_1d;
    unsigned int payload_1e;
    unsigned int rsvd_4;
    unsigned int swack_flag;
    unsigned int rsvd_5;
    unsigned int rsvd_6;
    unsigned int int_both;
    unsigned int fairness;
    unsigned int multilevel;
    unsigned int chaining;
    unsigned int rsvd_7;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

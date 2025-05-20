# Struct: <code>ptp_header</code>

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
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ptp_header {
    u8 tsmt;
    u8 ver;
    __be16 message_length;
    u8 domain_number;
    u8 reserved1;
    u8 flag_field[2];
    __be64 correction;
    __be32 reserved2;
    struct port_identity source_port_identity;
    __be16 sequence_id;
    u8 control;
    u8 log_message_interval;
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

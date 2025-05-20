# Struct: <code>usb_cdc_parsed_header</code>

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
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
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
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
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
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_cdc_parsed_header {
    struct usb_cdc_union_desc *usb_cdc_union_desc;
    struct usb_cdc_header_desc *usb_cdc_header_desc;
    struct usb_cdc_call_mgmt_descriptor *usb_cdc_call_mgmt_descriptor;
    struct usb_cdc_acm_descriptor *usb_cdc_acm_descriptor;
    struct usb_cdc_country_functional_desc *usb_cdc_country_functional_desc;
    struct usb_cdc_network_terminal_desc *usb_cdc_network_terminal_desc;
    struct usb_cdc_ether_desc *usb_cdc_ether_desc;
    struct usb_cdc_dmm_desc *usb_cdc_dmm_desc;
    struct usb_cdc_mdlm_desc *usb_cdc_mdlm_desc;
    struct usb_cdc_mdlm_detail_desc *usb_cdc_mdlm_detail_desc;
    struct usb_cdc_obex_desc *usb_cdc_obex_desc;
    struct usb_cdc_ncm_desc *usb_cdc_ncm_desc;
    struct usb_cdc_mbim_desc *usb_cdc_mbim_desc;
    struct usb_cdc_mbim_extended_desc *usb_cdc_mbim_extended_desc;
    bool phonet_magic_present;
};
```
</details>
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

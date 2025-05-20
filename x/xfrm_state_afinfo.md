# Struct: <code>xfrm_state_afinfo</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    const struct xfrm_type_offload * type_offload_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    const struct xfrm_type_offload * type_offload_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    const struct xfrm_type_offload * type_offload_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    unsigned int family;
    unsigned int proto;
    __be16 eth_proto;
    struct module *owner;
    const struct xfrm_type * type_map[256];
    const struct xfrm_type_offload * type_offload_map[256];
    struct xfrm_mode * mode_map[5];
    int (*init_flags)(struct xfrm_state *);
    void (*init_tempsel)(struct xfrm_selector *, const struct flowi *);
    void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *);
    int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int);
    int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int);
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
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
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
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
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_state_afinfo {
    u8 family;
    u8 proto;
    const struct xfrm_type_offload *type_offload_esp;
    const struct xfrm_type *type_esp;
    const struct xfrm_type *type_ipip;
    const struct xfrm_type *type_ipip6;
    const struct xfrm_type *type_comp;
    const struct xfrm_type *type_ah;
    const struct xfrm_type *type_routing;
    const struct xfrm_type *type_dstopts;
    int (*output)(struct net *, struct sock *, struct sk_buff *);
    int (*output_finish)(struct sock *, struct sk_buff *);
    int (*extract_input)(struct xfrm_state *, struct sk_buff *);
    int (*extract_output)(struct xfrm_state *, struct sk_buff *);
    int (*transport_finish)(struct sk_buff *, int);
    void (*local_error)(struct sk_buff *, u32);
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct xfrm_type_offload * type_offload_map[256]</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>const struct xfrm_type_offload *type_offload_esp</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_esp</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_ipip</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_ipip6</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_comp</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_ah</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_routing</code>
</li>
<li>
<b>Field added. </b>
<code>const struct xfrm_type *type_dstopts</code>
</li>
<li>
<b>Field removed. </b>
<code>__be16 eth_proto</code>
</li>
<li>
<b>Field removed. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct xfrm_type * type_map[256]</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct xfrm_type_offload * type_offload_map[256]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xfrm_mode * mode_map[5]</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*init_flags)(struct xfrm_state *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*init_tempsel)(struct xfrm_selector *, const struct flowi *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*init_temprop)(struct xfrm_state *, const struct xfrm_tmpl *, const xfrm_address_t *, const xfrm_address_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*tmpl_sort)(struct xfrm_tmpl **, struct xfrm_tmpl **, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*state_sort)(struct xfrm_state **, struct xfrm_state **, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int family</code> ➡️ <code>u8 family</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int proto</code> ➡️ <code>u8 proto</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*output_finish)(struct sock *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*extract_input)(struct xfrm_state *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*extract_output)(struct xfrm_state *, struct sk_buff *)</code>
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

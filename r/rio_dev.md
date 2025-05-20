# Struct: <code>rio_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
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
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
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
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rio_dev {
    struct list_head global_list;
    struct list_head net_list;
    struct rio_net *net;
    bool do_enum;
    u16 did;
    u16 vid;
    u32 device_rev;
    u16 asm_did;
    u16 asm_vid;
    u16 asm_rev;
    u16 efptr;
    u32 pef;
    u32 swpinfo;
    u32 src_ops;
    u32 dst_ops;
    u32 comp_tag;
    u32 phys_efptr;
    u32 phys_rmap;
    u32 em_efptr;
    u64 dma_mask;
    struct rio_driver *driver;
    struct device dev;
    struct resource riores[16];
    int (*pwcback)(struct rio_dev *, union rio_pw_msg *, int);
    u16 destid;
    u8 hopcount;
    struct rio_dev *prev;
    atomic_t state;
    struct rio_switch rswitch[0];
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
<code>u32 phys_rmap</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t state</code>
</li>
</ul>
</details>
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

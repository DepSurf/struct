# Struct: <code>vgasr_priv</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    struct dentry *switch_file;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
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
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vgasr_priv {
    bool active;
    bool delayed_switch_active;
    enum vga_switcheroo_client_id delayed_client_id;
    struct dentry *debugfs_root;
    int registered_clients;
    struct list_head clients;
    const struct vga_switcheroo_handler *handler;
    enum vga_switcheroo_handler_flags_t handler_flags;
    struct mutex mux_hw_lock;
    int old_ddc_owner;
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
<code>enum vga_switcheroo_handler_flags_t handler_flags</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex mux_hw_lock</code>
</li>
<li>
<b>Field added. </b>
<code>int old_ddc_owner</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct dentry *switch_file</code>
</li>
</ul>
</details>
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

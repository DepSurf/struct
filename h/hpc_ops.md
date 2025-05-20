# Struct: <code>hpc_ops</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
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
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
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
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hpc_ops {
    int (*power_on_slot)(struct slot *);
    int (*slot_enable)(struct slot *);
    int (*slot_disable)(struct slot *);
    int (*set_bus_speed_mode)(struct slot *, enum pci_bus_speed);
    int (*get_power_status)(struct slot *, u8 *);
    int (*get_attention_status)(struct slot *, u8 *);
    int (*set_attention_status)(struct slot *, u8);
    int (*get_latch_status)(struct slot *, u8 *);
    int (*get_adapter_status)(struct slot *, u8 *);
    int (*get_adapter_speed)(struct slot *, enum pci_bus_speed *);
    int (*get_mode1_ECC_cap)(struct slot *, u8 *);
    int (*get_prog_int)(struct slot *, u8 *);
    int (*query_power_fault)(struct slot *);
    void (*green_led_on)(struct slot *);
    void (*green_led_off)(struct slot *);
    void (*green_led_blink)(struct slot *);
    void (*release_ctlr)(struct controller *);
    int (*check_cmd_status)(struct controller *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*get_mode1_ECC_cap)(struct slot *, u8 *)</code>
</li>
</ul>
</details>
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

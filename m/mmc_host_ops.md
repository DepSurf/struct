# Struct: <code>mmc_host_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *, bool);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *, bool);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*execute_hs400_tuning)(struct mmc_host *, struct mmc_card *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*card_hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*execute_hs400_tuning)(struct mmc_host *, struct mmc_card *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*card_hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*execute_hs400_tuning)(struct mmc_host *, struct mmc_card *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*card_hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    int (*request_atomic)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*execute_hs400_tuning)(struct mmc_host *, struct mmc_card *);
    int (*prepare_sd_hs_tuning)(struct mmc_host *, struct mmc_card *);
    int (*execute_sd_hs_tuning)(struct mmc_host *, struct mmc_card *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*card_hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
    int (*init_sd_express)(struct mmc_host *, struct mmc_ios *);
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
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
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
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmc_host_ops {
    void (*post_req)(struct mmc_host *, struct mmc_request *, int);
    void (*pre_req)(struct mmc_host *, struct mmc_request *);
    void (*request)(struct mmc_host *, struct mmc_request *);
    void (*set_ios)(struct mmc_host *, struct mmc_ios *);
    int (*get_ro)(struct mmc_host *);
    int (*get_cd)(struct mmc_host *);
    void (*enable_sdio_irq)(struct mmc_host *, int);
    void (*ack_sdio_irq)(struct mmc_host *);
    void (*init_card)(struct mmc_host *, struct mmc_card *);
    int (*start_signal_voltage_switch)(struct mmc_host *, struct mmc_ios *);
    int (*card_busy)(struct mmc_host *);
    int (*execute_tuning)(struct mmc_host *, u32);
    int (*prepare_hs400_tuning)(struct mmc_host *, struct mmc_ios *);
    int (*hs400_prepare_ddr)(struct mmc_host *);
    void (*hs400_downgrade)(struct mmc_host *);
    void (*hs400_complete)(struct mmc_host *);
    void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *);
    int (*select_drive_strength)(struct mmc_card *, unsigned int, int, int, int *);
    void (*hw_reset)(struct mmc_host *);
    void (*card_event)(struct mmc_host *);
    int (*multi_io_quirk)(struct mmc_card *, unsigned int, int);
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
<code>void (*hs400_enhanced_strobe)(struct mmc_host *, struct mmc_ios *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*pre_req)(struct mmc_host *, struct mmc_request *, bool)</code> ➡️ <code>void (*pre_req)(struct mmc_host *, struct mmc_request *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*ack_sdio_irq)(struct mmc_host *)</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*hs400_prepare_ddr)(struct mmc_host *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*hs400_downgrade)(struct mmc_host *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*hs400_complete)(struct mmc_host *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*request_atomic)(struct mmc_host *, struct mmc_request *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*init_sd_express)(struct mmc_host *, struct mmc_ios *)</code>
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
<code>int (*execute_hs400_tuning)(struct mmc_host *, struct mmc_card *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*card_hw_reset)(struct mmc_host *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*hw_reset)(struct mmc_host *)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*prepare_sd_hs_tuning)(struct mmc_host *, struct mmc_card *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*execute_sd_hs_tuning)(struct mmc_host *, struct mmc_card *)</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

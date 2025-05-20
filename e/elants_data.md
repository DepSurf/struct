# Struct: <code>elants_data</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    u8 buf[169];
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    u8 buf[169];
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    u8 buf[169];
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    u8 buf[169];
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    unsigned int phy_x;
    unsigned int phy_y;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_chip_id chip_id;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    unsigned int phy_x;
    unsigned int phy_y;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_chip_id chip_id;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    unsigned int phy_x;
    unsigned int phy_y;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_chip_id chip_id;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    unsigned int phy_x;
    unsigned int phy_y;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_chip_id chip_id;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    unsigned int phy_x;
    unsigned int phy_y;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_chip_id chip_id;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    u8 major_res;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    unsigned int phy_x;
    unsigned int phy_y;
    struct touchscreen_properties prop;
    enum elants_state state;
    enum elants_chip_id chip_id;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool keep_power_in_suspend;
    u8 buf[169];
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct elants_data {
    struct i2c_client *client;
    struct input_dev *input;
    struct regulator *vcc33;
    struct regulator *vccio;
    struct gpio_desc *reset_gpio;
    u16 fw_version;
    u8 test_version;
    u8 solution_version;
    u8 bc_version;
    u8 iap_version;
    u16 hw_version;
    unsigned int x_res;
    unsigned int y_res;
    unsigned int x_max;
    unsigned int y_max;
    enum elants_state state;
    enum elants_iap_mode iap_mode;
    struct mutex sysfs_mutex;
    u8 cmd_resp[4];
    struct completion cmd_done;
    bool wake_irq_enabled;
    bool keep_power_in_suspend;
    u8 buf[169];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct touchscreen_properties prop</code>
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
<code>u8 major_res</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int phy_x</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int phy_y</code>
</li>
<li>
<b>Field added. </b>
<code>enum elants_chip_id chip_id</code>
</li>
</ul>
</details>
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
<code>bool wake_irq_enabled</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

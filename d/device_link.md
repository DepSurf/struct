# Struct: <code>device_link</code>

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
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    bool rpm_active;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    bool rpm_active;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    bool rpm_active;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    bool rpm_active;
    struct kref kref;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    bool rpm_active;
    struct kref kref;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct work_struct rm_work;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct work_struct rm_work;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct work_struct rm_work;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct work_struct rm_work;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct work_struct rm_work;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    struct device link_dev;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct work_struct rm_work;
    bool supplier_preactivated;
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
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
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
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct device_link {
    struct device *supplier;
    struct list_head s_node;
    struct device *consumer;
    struct list_head c_node;
    enum device_link_state status;
    u32 flags;
    refcount_t rpm_active;
    struct kref kref;
    struct callback_head callback_head;
    bool supplier_preactivated;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kref kref</code>
</li>
</ul>
</details>
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
<code>bool supplier_preactivated</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool rpm_active</code> ➡️ <code>refcount_t rpm_active</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device link_dev</code>
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
<code>struct work_struct rm_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head callback_head</code>
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

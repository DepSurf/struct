# Struct: <code>virtio_config_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const char **);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, int);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, int);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, int);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    void (*synchronize_cbs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    void (*synchronize_cbs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
    int (*disable_vq_and_reset)(struct virtqueue *);
    int (*enable_vq_after_reset)(struct virtqueue *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    void (*synchronize_cbs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
    int (*disable_vq_and_reset)(struct virtqueue *);
    int (*enable_vq_after_reset)(struct virtqueue *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    void (*synchronize_cbs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
    bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8);
    int (*disable_vq_and_reset)(struct virtqueue *);
    int (*enable_vq_after_reset)(struct virtqueue *);
    int (*create_avq)(struct virtio_device *);
    void (*destroy_avq)(struct virtio_device *);
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
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
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
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct virtio_config_ops {
    void (*get)(struct virtio_device *, unsigned int, void *, unsigned int);
    void (*set)(struct virtio_device *, unsigned int, const void *, unsigned int);
    u32 (*generation)(struct virtio_device *);
    u8 (*get_status)(struct virtio_device *);
    void (*set_status)(struct virtio_device *, u8);
    void (*reset)(struct virtio_device *);
    int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *);
    void (*del_vqs)(struct virtio_device *);
    u64 (*get_features)(struct virtio_device *);
    int (*finalize_features)(struct virtio_device *);
    const char * (*bus_name)(struct virtio_device *);
    int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *);
    const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int);
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
<b>Field type changed. </b>
<code>int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const char **)</code> ➡️ <code>int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *)</code>
</li>
</ul>
</details>
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
<code>const struct cpumask * (*get_vq_affinity)(struct virtio_device *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *)</code> ➡️ <code>int (*find_vqs)(struct virtio_device *, unsigned int, struct virtqueue **, vq_callback_t **, const const char * *, const bool *, struct irq_affinity *)</code>
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
<b>Field type changed. </b>
<code>int (*set_vq_affinity)(struct virtqueue *, int)</code> ➡️ <code>int (*set_vq_affinity)(struct virtqueue *, const struct cpumask *)</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*get_shm_region)(struct virtio_device *, struct virtio_shm_region *, u8)</code>
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
<code>void (*synchronize_cbs)(struct virtio_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*disable_vq_and_reset)(struct virtqueue *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*enable_vq_after_reset)(struct virtqueue *)</code>
</li>
</ul>
</details>
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
<code>int (*create_avq)(struct virtio_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*destroy_avq)(struct virtio_device *)</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

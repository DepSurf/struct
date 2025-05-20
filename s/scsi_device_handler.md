# Struct: <code>scsi_device_handler</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    int (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    int (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    int (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    int (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    int (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    int (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
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
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
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
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct scsi_device_handler {
    struct list_head list;
    struct module *module;
    const char *name;
    int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *);
    int (*attach)(struct scsi_device *);
    void (*detach)(struct scsi_device *);
    int (*activate)(struct scsi_device *, activate_complete, void *);
    blk_status_t (*prep_fn)(struct scsi_device *, struct request *);
    int (*set_params)(struct scsi_device *, const char *);
    void (*rescan)(struct scsi_device *);
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
<code>void (*rescan)(struct scsi_device *)</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*prep_fn)(struct scsi_device *, struct request *)</code> ➡️ <code>blk_status_t (*prep_fn)(struct scsi_device *, struct request *)</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *)</code> ➡️ <code>enum scsi_disposition (*check_sense)(struct scsi_device *, struct scsi_sense_hdr *)</code>
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

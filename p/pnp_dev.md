# Struct: <code>pnp_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
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
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
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
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pnp_dev {
    struct device dev;
    u64 dma_mask;
    unsigned int number;
    int status;
    struct list_head global_list;
    struct list_head protocol_list;
    struct list_head card_list;
    struct list_head rdev_list;
    struct pnp_protocol *protocol;
    struct pnp_card *card;
    struct pnp_driver *driver;
    struct pnp_card_link *card_link;
    struct pnp_id *id;
    int active;
    int capabilities;
    unsigned int num_dependent_sets;
    struct list_head resources;
    struct list_head options;
    char name[50];
    int flags;
    struct proc_dir_entry *procent;
    void *data;
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

# Struct: <code>md_personality</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    void (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    void (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    void (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*prepare_suspend)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*change_consistency_policy)(struct mddev *, const char *);
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
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
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
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct md_personality {
    char *name;
    int level;
    struct list_head list;
    struct module *owner;
    bool (*make_request)(struct mddev *, struct bio *);
    int (*run)(struct mddev *);
    int (*start)(struct mddev *);
    void (*free)(struct mddev *, void *);
    void (*status)(struct seq_file *, struct mddev *);
    void (*error_handler)(struct mddev *, struct md_rdev *);
    int (*hot_add_disk)(struct mddev *, struct md_rdev *);
    int (*hot_remove_disk)(struct mddev *, struct md_rdev *);
    int (*spare_active)(struct mddev *);
    sector_t (*sync_request)(struct mddev *, sector_t, int *);
    int (*resize)(struct mddev *, sector_t);
    sector_t (*size)(struct mddev *, sector_t, int);
    int (*check_reshape)(struct mddev *);
    int (*start_reshape)(struct mddev *);
    void (*finish_reshape)(struct mddev *);
    void (*update_reshape_pos)(struct mddev *);
    void (*quiesce)(struct mddev *, int);
    void * (*takeover)(struct mddev *);
    int (*congested)(struct mddev *, int);
    int (*change_consistency_policy)(struct mddev *, const char *);
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
<code>int (*change_consistency_policy)(struct mddev *, const char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*make_request)(struct mddev *, struct bio *)</code> ➡️ <code>bool (*make_request)(struct mddev *, struct bio *)</code>
</li>
</ul>
</details>
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
<code>int (*start)(struct mddev *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*update_reshape_pos)(struct mddev *)</code>
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
<b>Field removed. </b>
<code>int (*congested)(struct mddev *, int)</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*prepare_suspend)(struct mddev *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*prepare_suspend)(struct mddev *)</code>
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

# Struct: <code>key_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
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
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
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
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct key_type {
    const char *name;
    size_t def_datalen;
    unsigned int flags;
    int (*vet_description)(const char *);
    int (*preparse)(struct key_preparsed_payload *);
    void (*free_preparse)(struct key_preparsed_payload *);
    int (*instantiate)(struct key *, struct key_preparsed_payload *);
    int (*update)(struct key *, struct key_preparsed_payload *);
    int (*match_preparse)(struct key_match_data *);
    void (*match_free)(struct key_match_data *);
    void (*revoke)(struct key *);
    void (*destroy)(struct key *);
    void (*describe)(const struct key *, struct seq_file *);
    long int (*read)(const struct key *, char *, size_t);
    request_key_actor_t request_key;
    struct key_restriction * (*lookup_restriction)(const char *);
    int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *);
    int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *);
    int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *);
    struct list_head link;
    struct lock_class_key lock_class;
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
<code>struct key_restriction * (*lookup_restriction)(const char *)</code>
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
<code>int (*asym_query)(const struct kernel_pkey_params *, struct kernel_pkey_query *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*asym_eds_op)(struct kernel_pkey_params *, const void *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*asym_verify_signature)(struct kernel_pkey_params *, const void *, const void *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int flags</code>
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

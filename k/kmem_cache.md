# Struct: <code>kmem_cache</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    long unsigned int flags;
    long unsigned int min_partial;
    int size;
    int object_size;
    int offset;
    int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    int inuse;
    int align;
    int reserved;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct memcg_cache_params memcg_params;
    int max_attr_size;
    struct kset *memcg_kset;
    int remote_node_defrag_ratio;
    struct kmem_cache_node * node[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    long unsigned int flags;
    long unsigned int min_partial;
    int size;
    int object_size;
    int offset;
    int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    int inuse;
    int align;
    int reserved;
    const char *name;
    struct list_head list;
    int red_left_pad;
    struct kobject kobj;
    struct memcg_cache_params memcg_params;
    int max_attr_size;
    struct kset *memcg_kset;
    int remote_node_defrag_ratio;
    unsigned int *random_seq;
    struct kmem_cache_node * node[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    long unsigned int flags;
    long unsigned int min_partial;
    int size;
    int object_size;
    int offset;
    int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    int inuse;
    int align;
    int reserved;
    const char *name;
    struct list_head list;
    int red_left_pad;
    struct kobject kobj;
    struct memcg_cache_params memcg_params;
    int max_attr_size;
    struct kset *memcg_kset;
    int remote_node_defrag_ratio;
    unsigned int *random_seq;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    long unsigned int flags;
    long unsigned int min_partial;
    int size;
    int object_size;
    int offset;
    int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    int inuse;
    int align;
    int reserved;
    int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    int max_attr_size;
    struct kset *memcg_kset;
    int remote_node_defrag_ratio;
    unsigned int *random_seq;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    int size;
    int object_size;
    int offset;
    int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    int inuse;
    int align;
    int reserved;
    int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    int remote_node_defrag_ratio;
    unsigned int *random_seq;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    unsigned int cpu_partial_slabs;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    unsigned int cpu_partial_slabs;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    unsigned int cpu_partial_slabs;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    struct reciprocal_value reciprocal_size;
    unsigned int offset;
    unsigned int cpu_partial;
    unsigned int cpu_partial_slabs;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
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
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1];
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
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kmem_cache {
    struct kmem_cache_cpu *cpu_slab;
    slab_flags_t flags;
    long unsigned int min_partial;
    unsigned int size;
    unsigned int object_size;
    unsigned int offset;
    unsigned int cpu_partial;
    struct kmem_cache_order_objects oo;
    struct kmem_cache_order_objects max;
    struct kmem_cache_order_objects min;
    gfp_t allocflags;
    int refcount;
    void (*ctor)(void *);
    unsigned int inuse;
    unsigned int align;
    unsigned int red_left_pad;
    const char *name;
    struct list_head list;
    struct kobject kobj;
    struct work_struct kobj_remove_work;
    struct memcg_cache_params memcg_params;
    unsigned int max_attr_size;
    struct kset *memcg_kset;
    long unsigned int random;
    unsigned int remote_node_defrag_ratio;
    unsigned int *random_seq;
    unsigned int useroffset;
    unsigned int usersize;
    struct kmem_cache_node * node[1024];
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
<code>int red_left_pad</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int *random_seq</code>
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
<code>struct kmem_cache_node * node[64]</code> ➡️ <code>struct kmem_cache_node * node[1024]</code>
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
<code>struct work_struct kobj_remove_work</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int random</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int flags</code> ➡️ <code>slab_flags_t flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int useroffset</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int usersize</code>
</li>
<li>
<b>Field removed. </b>
<code>int reserved</code>
</li>
<li>
<b>Field type changed. </b>
<code>int size</code> ➡️ <code>unsigned int size</code>
</li>
<li>
<b>Field type changed. </b>
<code>int object_size</code> ➡️ <code>unsigned int object_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>int offset</code> ➡️ <code>unsigned int offset</code>
</li>
<li>
<b>Field type changed. </b>
<code>int cpu_partial</code> ➡️ <code>unsigned int cpu_partial</code>
</li>
<li>
<b>Field type changed. </b>
<code>int inuse</code> ➡️ <code>unsigned int inuse</code>
</li>
<li>
<b>Field type changed. </b>
<code>int align</code> ➡️ <code>unsigned int align</code>
</li>
<li>
<b>Field type changed. </b>
<code>int red_left_pad</code> ➡️ <code>unsigned int red_left_pad</code>
</li>
<li>
<b>Field type changed. </b>
<code>int max_attr_size</code> ➡️ <code>unsigned int max_attr_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>int remote_node_defrag_ratio</code> ➡️ <code>unsigned int remote_node_defrag_ratio</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct reciprocal_value reciprocal_size</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct kobj_remove_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct memcg_cache_params memcg_params</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int max_attr_size</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kset *memcg_kset</code>
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
<code>unsigned int cpu_partial_slabs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kmem_cache_order_objects max</code>
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct kmem_cache_node * node[1024]</code> ➡️ <code>struct kmem_cache_node * node[64]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int remote_node_defrag_ratio</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct kmem_cache_node * node[1024]</code> ➡️ <code>struct kmem_cache_node * node[1]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct kmem_cache_node * node[1024]</code> ➡️ <code>struct kmem_cache_node * node[256]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int remote_node_defrag_ratio</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct kmem_cache_node * node[1024]</code> ➡️ <code>struct kmem_cache_node * node[1]</code>
</li>
</ul>
</details>
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

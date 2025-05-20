# Struct: <code>rio_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u32, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
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
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
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
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rio_ops {
    int (*lcread)(struct rio_mport *, int, u32, int, u32 *);
    int (*lcwrite)(struct rio_mport *, int, u32, int, u32);
    int (*cread)(struct rio_mport *, int, u16, u8, u32, int, u32 *);
    int (*cwrite)(struct rio_mport *, int, u16, u8, u32, int, u32);
    int (*dsend)(struct rio_mport *, int, u16, u16);
    int (*pwenable)(struct rio_mport *, int);
    int (*open_outb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_outb_mbox)(struct rio_mport *, int);
    int (*open_inb_mbox)(struct rio_mport *, void *, int, int);
    void (*close_inb_mbox)(struct rio_mport *, int);
    int (*add_outb_message)(struct rio_mport *, struct rio_dev *, int, void *, size_t);
    int (*add_inb_buffer)(struct rio_mport *, int, void *);
    void * (*get_inb_message)(struct rio_mport *, int);
    int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32);
    void (*unmap_inb)(struct rio_mport *, dma_addr_t);
    int (*query_mport)(struct rio_mport *, struct rio_mport_attr *);
    int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *);
    void (*unmap_outb)(struct rio_mport *, u16, u64);
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
<code>int (*query_mport)(struct rio_mport *, struct rio_mport_attr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_outb)(struct rio_mport *, u16, u64, u32, u32, dma_addr_t *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unmap_outb)(struct rio_mport *, u16, u64)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u32, u32)</code> ➡️ <code>int (*map_inb)(struct rio_mport *, dma_addr_t, u64, u64, u32)</code>
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

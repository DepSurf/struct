# Struct: <code>usb_ep_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
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
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
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
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
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
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_ep_ops {
    int (*enable)(struct usb_ep *, const struct usb_endpoint_descriptor *);
    int (*disable)(struct usb_ep *);
    void (*dispose)(struct usb_ep *);
    struct usb_request * (*alloc_request)(struct usb_ep *, gfp_t);
    void (*free_request)(struct usb_ep *, struct usb_request *);
    int (*queue)(struct usb_ep *, struct usb_request *, gfp_t);
    int (*dequeue)(struct usb_ep *, struct usb_request *);
    int (*set_halt)(struct usb_ep *, int);
    int (*set_wedge)(struct usb_ep *);
    int (*fifo_status)(struct usb_ep *);
    void (*fifo_flush)(struct usb_ep *);
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*dispose)(struct usb_ep *)</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>

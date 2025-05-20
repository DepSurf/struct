# Struct: <code>dma_async_tx_descriptor</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    enum dma_desc_metadata_mode desc_metadata_mode;
    struct dma_descriptor_metadata_ops *metadata_ops;
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
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    struct dma_async_tx_descriptor *next;
    struct dma_async_tx_descriptor *parent;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
    struct dma_async_tx_descriptor *next;
    struct dma_async_tx_descriptor *parent;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
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
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dma_async_tx_descriptor {
    dma_cookie_t cookie;
    enum dma_ctrl_flags flags;
    dma_addr_t phys;
    struct dma_chan *chan;
    dma_cookie_t (*tx_submit)(struct dma_async_tx_descriptor *);
    int (*desc_free)(struct dma_async_tx_descriptor *);
    dma_async_tx_callback callback;
    dma_async_tx_callback_result callback_result;
    void *callback_param;
    struct dmaengine_unmap_data *unmap;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>dma_async_tx_callback_result callback_result</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum dma_desc_metadata_mode desc_metadata_mode</code>
</li>
<li>
<b>Field added. </b>
<code>struct dma_descriptor_metadata_ops *metadata_ops</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dma_async_tx_descriptor *next</code>
</li>
<li>
<b>Field added. </b>
<code>struct dma_async_tx_descriptor *parent</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dma_async_tx_descriptor *next</code>
</li>
<li>
<b>Field added. </b>
<code>struct dma_async_tx_descriptor *parent</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
</ul>
</details>
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

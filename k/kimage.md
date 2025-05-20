# Struct: <code>kimage</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
    void *ima_buffer;
    phys_addr_t ima_buffer_addr;
    size_t ima_buffer_size;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
    void *ima_buffer;
    phys_addr_t ima_buffer_addr;
    size_t ima_buffer_size;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    unsigned int update_elfcorehdr;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
    int hp_action;
    int elfcorehdr_index;
    bool elfcorehdr_updated;
    void *ima_buffer;
    phys_addr_t ima_buffer_addr;
    size_t ima_buffer_size;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
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
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kimage {
    kimage_entry_t head;
    kimage_entry_t *entry;
    kimage_entry_t *last_entry;
    long unsigned int start;
    struct page *control_code_page;
    struct page *swap_page;
    void *vmcoreinfo_data_copy;
    long unsigned int nr_segments;
    struct kexec_segment segment[16];
    struct list_head control_pages;
    struct list_head dest_pages;
    struct list_head unusable_pages;
    long unsigned int control_page;
    unsigned int type;
    unsigned int preserve_context;
    unsigned int file_mode;
    struct kimage_arch arch;
    void *kernel_buf;
    long unsigned int kernel_buf_len;
    void *initrd_buf;
    long unsigned int initrd_buf_len;
    char *cmdline_buf;
    long unsigned int cmdline_buf_len;
    const struct kexec_file_ops *fops;
    void *image_loader_data;
    struct purgatory_info purgatory_info;
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
<code>void *vmcoreinfo_data_copy</code>
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
<b>Field type changed. </b>
<code>struct kexec_file_ops *fops</code> ➡️ <code>const struct kexec_file_ops *fops</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *elf_headers</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int elf_headers_sz</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int elf_load_addr</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *ima_buffer</code>
</li>
<li>
<b>Field added. </b>
<code>phys_addr_t ima_buffer_addr</code>
</li>
<li>
<b>Field added. </b>
<code>size_t ima_buffer_size</code>
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
<code>unsigned int update_elfcorehdr</code>
</li>
<li>
<b>Field added. </b>
<code>int hp_action</code>
</li>
<li>
<b>Field added. </b>
<code>int elfcorehdr_index</code>
</li>
<li>
<b>Field added. </b>
<code>bool elfcorehdr_updated</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void *kernel_buf</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int kernel_buf_len</code>
</li>
<li>
<b>Field removed. </b>
<code>void *initrd_buf</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int initrd_buf_len</code>
</li>
<li>
<b>Field removed. </b>
<code>char *cmdline_buf</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int cmdline_buf_len</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct kexec_file_ops *fops</code>
</li>
<li>
<b>Field removed. </b>
<code>void *image_loader_data</code>
</li>
<li>
<b>Field removed. </b>
<code>struct purgatory_info purgatory_info</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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

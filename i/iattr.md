# Struct: <code>iattr</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec ia_atime;
    struct timespec ia_mtime;
    struct timespec ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec ia_atime;
    struct timespec ia_mtime;
    struct timespec ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec ia_atime;
    struct timespec ia_mtime;
    struct timespec ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec ia_atime;
    struct timespec ia_mtime;
    struct timespec ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec ia_atime;
    struct timespec ia_mtime;
    struct timespec ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    vfsuid_t ia_vfsuid;
    kgid_t ia_gid;
    vfsgid_t ia_vfsgid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    vfsuid_t ia_vfsuid;
    kgid_t ia_gid;
    vfsgid_t ia_vfsgid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    vfsuid_t ia_vfsuid;
    kgid_t ia_gid;
    vfsgid_t ia_vfsgid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
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
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
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
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iattr {
    unsigned int ia_valid;
    umode_t ia_mode;
    kuid_t ia_uid;
    kgid_t ia_gid;
    loff_t ia_size;
    struct timespec64 ia_atime;
    struct timespec64 ia_mtime;
    struct timespec64 ia_ctime;
    struct file *ia_file;
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
<b>Field type changed. </b>
<code>struct timespec ia_atime</code> ➡️ <code>struct timespec64 ia_atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timespec ia_mtime</code> ➡️ <code>struct timespec64 ia_mtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timespec ia_ctime</code> ➡️ <code>struct timespec64 ia_ctime</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>vfsuid_t ia_vfsuid</code>
</li>
<li>
<b>Field added. </b>
<code>vfsgid_t ia_vfsgid</code>
</li>
</ul>
</details>
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

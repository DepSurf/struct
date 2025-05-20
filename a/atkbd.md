# Struct: <code>atkbd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    u32 function_row_physmap[24];
    int num_function_row_keys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    u32 function_row_physmap[24];
    int num_function_row_keys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    u32 function_row_physmap[24];
    int num_function_row_keys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    u32 function_row_physmap[24];
    int num_function_row_keys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    struct vivaldi_data vdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    struct vivaldi_data vdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    struct vivaldi_data vdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
    struct vivaldi_data vdata;
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
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[16];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
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
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct atkbd {
    struct ps2dev ps2dev;
    struct input_dev *dev;
    char name[64];
    char phys[32];
    short unsigned int id;
    short unsigned int keycode[512];
    long unsigned int force_release_mask[8];
    unsigned char set;
    bool translated;
    bool extra;
    bool write;
    bool softrepeat;
    bool softraw;
    bool scroll;
    bool enabled;
    unsigned char emul;
    bool resend;
    bool release;
    long unsigned int xl_bit;
    unsigned int last;
    long unsigned int time;
    long unsigned int err_count;
    struct delayed_work event_work;
    long unsigned int event_jiffies;
    long unsigned int event_mask;
    struct mutex mutex;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 function_row_physmap[24]</code>
</li>
<li>
<b>Field added. </b>
<code>int num_function_row_keys</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct vivaldi_data vdata</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 function_row_physmap[24]</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_function_row_keys</code>
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
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int force_release_mask[8]</code> ➡️ <code>long unsigned int force_release_mask[16]</code>
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

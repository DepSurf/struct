# Struct: <code>irq_bypass_consumer</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct irq_bypass_consumer {
    struct list_head node;
    void *token;
    int (*add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*stop)(struct irq_bypass_consumer *);
    void (*start)(struct irq_bypass_consumer *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
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

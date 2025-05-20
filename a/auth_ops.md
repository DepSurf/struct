# Struct: <code>auth_ops</code>

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
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct auth_ops {
    char *name;
    struct module *owner;
    int flavour;
    int (*accept)(struct svc_rqst *);
    int (*release)(struct svc_rqst *);
    void (*domain_release)(struct auth_domain *);
    int (*set_client)(struct svc_rqst *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct auth_ops {
    char *name;
    struct module *owner;
    int flavour;
    int (*accept)(struct svc_rqst *);
    int (*release)(struct svc_rqst *);
    void (*domain_release)(struct auth_domain *);
    int (*set_client)(struct svc_rqst *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct auth_ops {
    char *name;
    struct module *owner;
    int flavour;
    int (*accept)(struct svc_rqst *);
    int (*release)(struct svc_rqst *);
    void (*domain_release)(struct auth_domain *);
    int (*set_client)(struct svc_rqst *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct auth_ops {
    char *name;
    struct module *owner;
    int flavour;
    int (*accept)(struct svc_rqst *);
    int (*release)(struct svc_rqst *);
    void (*domain_release)(struct auth_domain *);
    int (*set_client)(struct svc_rqst *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct auth_ops {
    char *name;
    struct module *owner;
    int flavour;
    enum svc_auth_status (*accept)(struct svc_rqst *);
    int (*release)(struct svc_rqst *);
    void (*domain_release)(struct auth_domain *);
    enum svc_auth_status (*set_client)(struct svc_rqst *);
    rpc_authflavor_t (*pseudoflavor)(struct svc_rqst *);
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
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
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>rpc_authflavor_t (*pseudoflavor)(struct svc_rqst *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*accept)(struct svc_rqst *)</code> ➡️ <code>enum svc_auth_status (*accept)(struct svc_rqst *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_client)(struct svc_rqst *)</code> ➡️ <code>enum svc_auth_status (*set_client)(struct svc_rqst *)</code>
</li>
</ul>
</details>
</li>
</ul>

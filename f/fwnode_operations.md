# Struct: <code>fwnode_operations</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fwnode_operations {
    void (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(struct fwnode_handle *);
    bool (*property_present)(struct fwnode_handle *, const char *);
    int (*property_read_int_array)(struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(struct fwnode_handle *, const char *);
    struct fwnode_handle * (*graph_get_next_endpoint)(struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    int (*add_links)(const struct fwnode_handle *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    int (*add_links)(struct fwnode_handle *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    int (*add_links)(struct fwnode_handle *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    int (*add_links)(struct fwnode_handle *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*device_dma_supported)(const struct fwnode_handle *);
    enum dev_dma_attr (*device_get_dma_attr)(const struct fwnode_handle *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    void * (*iomap)(struct fwnode_handle *, int);
    int (*irq_get)(const struct fwnode_handle *, unsigned int);
    int (*add_links)(struct fwnode_handle *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*device_dma_supported)(const struct fwnode_handle *);
    enum dev_dma_attr (*device_get_dma_attr)(const struct fwnode_handle *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    void * (*iomap)(struct fwnode_handle *, int);
    int (*irq_get)(const struct fwnode_handle *, unsigned int);
    int (*add_links)(struct fwnode_handle *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*device_dma_supported)(const struct fwnode_handle *);
    enum dev_dma_attr (*device_get_dma_attr)(const struct fwnode_handle *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    void * (*iomap)(struct fwnode_handle *, int);
    int (*irq_get)(const struct fwnode_handle *, unsigned int);
    int (*add_links)(struct fwnode_handle *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*device_dma_supported)(const struct fwnode_handle *);
    enum dev_dma_attr (*device_get_dma_attr)(const struct fwnode_handle *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    const char * (*get_name)(const struct fwnode_handle *);
    const char * (*get_name_prefix)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
    void * (*iomap)(struct fwnode_handle *, int);
    int (*irq_get)(const struct fwnode_handle *, unsigned int);
    int (*add_links)(struct fwnode_handle *);
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
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
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
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fwnode_operations {
    struct fwnode_handle * (*get)(struct fwnode_handle *);
    void (*put)(struct fwnode_handle *);
    bool (*device_is_available)(const struct fwnode_handle *);
    const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *);
    bool (*property_present)(const struct fwnode_handle *, const char *);
    int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t);
    int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t);
    struct fwnode_handle * (*get_parent)(const struct fwnode_handle *);
    struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *);
    int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *);
    struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *);
    struct fwnode_handle * (*graph_get_port_parent)(struct fwnode_handle *);
    int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *);
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_reference_args)(const struct fwnode_handle *, const char *, const char *, unsigned int, unsigned int, struct fwnode_reference_args *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get)(struct fwnode_handle *)</code> ➡️ <code>struct fwnode_handle * (*get)(struct fwnode_handle *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*device_is_available)(struct fwnode_handle *)</code> ➡️ <code>bool (*device_is_available)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*property_present)(struct fwnode_handle *, const char *)</code> ➡️ <code>bool (*property_present)(const struct fwnode_handle *, const char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*property_read_int_array)(struct fwnode_handle *, const char *, unsigned int, void *, size_t)</code> ➡️ <code>int (*property_read_int_array)(const struct fwnode_handle *, const char *, unsigned int, void *, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*property_read_string_array)(struct fwnode_handle *, const char *, const char **, size_t)</code> ➡️ <code>int (*property_read_string_array)(const struct fwnode_handle *, const char *, const char **, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fwnode_handle * (*get_parent)(struct fwnode_handle *)</code> ➡️ <code>struct fwnode_handle * (*get_parent)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fwnode_handle * (*get_next_child_node)(struct fwnode_handle *, struct fwnode_handle *)</code> ➡️ <code>struct fwnode_handle * (*get_next_child_node)(const struct fwnode_handle *, struct fwnode_handle *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fwnode_handle * (*get_named_child_node)(struct fwnode_handle *, const char *)</code> ➡️ <code>struct fwnode_handle * (*get_named_child_node)(const struct fwnode_handle *, const char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fwnode_handle * (*graph_get_next_endpoint)(struct fwnode_handle *, struct fwnode_handle *)</code> ➡️ <code>struct fwnode_handle * (*graph_get_next_endpoint)(const struct fwnode_handle *, struct fwnode_handle *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fwnode_handle * (*graph_get_remote_endpoint)(struct fwnode_handle *)</code> ➡️ <code>struct fwnode_handle * (*graph_get_remote_endpoint)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*graph_parse_endpoint)(struct fwnode_handle *, struct fwnode_endpoint *)</code> ➡️ <code>int (*graph_parse_endpoint)(const struct fwnode_handle *, struct fwnode_endpoint *)</code>
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
<code>const void * (*device_get_match_data)(const struct fwnode_handle *, const struct device *)</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char * (*get_name)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field added. </b>
<code>const char * (*get_name_prefix)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*add_links)(const struct fwnode_handle *, struct device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*add_links)(const struct fwnode_handle *, struct device *)</code> ➡️ <code>int (*add_links)(struct fwnode_handle *)</code>
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
<code>bool (*device_dma_supported)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field added. </b>
<code>enum dev_dma_attr (*device_get_dma_attr)(const struct fwnode_handle *)</code>
</li>
<li>
<b>Field added. </b>
<code>void * (*iomap)(struct fwnode_handle *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*irq_get)(const struct fwnode_handle *, unsigned int)</code>
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

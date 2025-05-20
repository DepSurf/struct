# Struct: <code>policydb</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[7];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[7];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[7];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    struct flex_array * sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct flex_array *type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct flex_array *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct_array;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct hashtab role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab filename_trans;
    u32 compat_filename_trans_count;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    u32 cond_list_len;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
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
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
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
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct policydb {
    int mls_enabled;
    struct symtab symtab[8];
    char ** sym_val_to_name[8];
    struct class_datum **class_val_to_struct;
    struct role_datum **role_val_to_struct;
    struct user_datum **user_val_to_struct;
    struct type_datum **type_val_to_struct;
    struct avtab te_avtab;
    struct role_trans *role_tr;
    struct ebitmap filename_trans_ttypes;
    struct hashtab *filename_trans;
    struct cond_bool_datum **bool_val_to_struct;
    struct avtab te_cond_avtab;
    struct cond_node *cond_list;
    struct role_allow *role_allow;
    struct ocontext * ocontexts[9];
    struct genfs *genfs;
    struct hashtab *range_tr;
    struct ebitmap *type_attr_map_array;
    struct ebitmap policycaps;
    struct ebitmap permissive_map;
    size_t len;
    unsigned int policyvers;
    unsigned int reject_unknown;
    unsigned int allow_unknown;
    u16 process_class;
    u32 process_trans_perms;
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
<b>Field type changed. </b>
<code>struct ocontext * ocontexts[7]</code> ➡️ <code>struct ocontext * ocontexts[9]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct flex_array * sym_val_to_name[8]</code> ➡️ <code>char ** sym_val_to_name[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct flex_array *type_val_to_struct_array</code> ➡️ <code>struct type_datum **type_val_to_struct_array</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct flex_array *type_attr_map_array</code> ➡️ <code>struct ebitmap *type_attr_map_array</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct type_datum **type_val_to_struct</code>
</li>
<li>
<b>Field removed. </b>
<code>struct type_datum **type_val_to_struct_array</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 compat_filename_trans_count</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cond_list_len</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct role_trans *role_tr</code> ➡️ <code>struct hashtab role_tr</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hashtab *filename_trans</code> ➡️ <code>struct hashtab filename_trans</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hashtab *range_tr</code> ➡️ <code>struct hashtab range_tr</code>
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

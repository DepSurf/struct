# Struct: <code>nfs_rpc_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, const struct qstr *);
    void (*unlink_setup)(struct rpc_message *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct inode *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, int);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, int);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    int (*return_delegation)(struct inode *);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, const struct qstr *);
    void (*unlink_setup)(struct rpc_message *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct inode *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, int);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, int);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    int (*return_delegation)(struct inode *);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, const struct qstr *);
    void (*unlink_setup)(struct rpc_message *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct inode *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    int (*return_delegation)(struct inode *);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, const struct qstr *);
    void (*unlink_setup)(struct rpc_message *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct inode *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    int (*return_delegation)(struct inode *);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*submount)(struct fs_context *, struct nfs_server *);
    int (*try_get_tree)(struct fs_context *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct nfs_readdir_arg *, struct nfs_readdir_res *);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct fs_context *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*submount)(struct fs_context *, struct nfs_server *);
    int (*try_get_tree)(struct fs_context *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct nfs_readdir_arg *, struct nfs_readdir_res *);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct fs_context *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
    int (*discover_trunking)(struct nfs_server *, struct nfs_fh *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*submount)(struct fs_context *, struct nfs_server *);
    int (*try_get_tree)(struct fs_context *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *);
    int (*access)(struct inode *, struct nfs_access_entry *, const struct cred *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct nfs_readdir_arg *, struct nfs_readdir_res *);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct fs_context *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
    int (*discover_trunking)(struct nfs_server *, struct nfs_fh *);
    void (*enable_swap)(struct inode *);
    void (*disable_swap)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*submount)(struct fs_context *, struct nfs_server *);
    int (*try_get_tree)(struct fs_context *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *);
    int (*access)(struct inode *, struct nfs_access_entry *, const struct cred *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct nfs_readdir_arg *, struct nfs_readdir_res *);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct fs_context *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
    int (*discover_trunking)(struct nfs_server *, struct nfs_fh *);
    void (*enable_swap)(struct inode *);
    void (*disable_swap)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*submount)(struct fs_context *, struct nfs_server *);
    int (*try_get_tree)(struct fs_context *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *);
    int (*access)(struct inode *, struct nfs_access_entry *, const struct cred *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct nfs_readdir_arg *, struct nfs_readdir_res *);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct fs_context *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
    int (*discover_trunking)(struct nfs_server *, struct nfs_fh *);
    void (*enable_swap)(struct inode *);
    void (*disable_swap)(struct inode *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*submount)(struct fs_context *, struct nfs_server *);
    int (*try_get_tree)(struct fs_context *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *);
    int (*access)(struct inode *, struct nfs_access_entry *, const struct cred *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct folio *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct nfs_readdir_arg *, struct nfs_readdir_res *);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct fs_context *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
    int (*discover_trunking)(struct nfs_server *, struct nfs_fh *);
    void (*enable_swap)(struct inode *);
    void (*disable_swap)(struct inode *);
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
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
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
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nfs_rpc_ops {
    u32 version;
    const struct dentry_operations *dentry_ops;
    const struct inode_operations *dir_inode_ops;
    const struct inode_operations *file_inode_ops;
    const struct file_operations *file_ops;
    const struct nlmclnt_operations *nlmclnt_ops;
    int (*getroot)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    struct vfsmount * (*submount)(struct nfs_server *, struct dentry *, struct nfs_fh *, struct nfs_fattr *);
    struct dentry * (*try_mount)(int, const char *, struct nfs_mount_info *, struct nfs_subversion *);
    int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *);
    int (*setattr)(struct dentry *, struct nfs_fattr *, struct iattr *);
    int (*lookup)(struct inode *, const struct qstr *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *);
    int (*access)(struct inode *, struct nfs_access_entry *);
    int (*readlink)(struct inode *, struct page *, unsigned int, unsigned int);
    int (*create)(struct inode *, struct dentry *, struct iattr *, int);
    int (*remove)(struct inode *, struct dentry *);
    void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *);
    void (*unlink_rpc_prepare)(struct rpc_task *, struct nfs_unlinkdata *);
    int (*unlink_done)(struct rpc_task *, struct inode *);
    void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *);
    void (*rename_rpc_prepare)(struct rpc_task *, struct nfs_renamedata *);
    int (*rename_done)(struct rpc_task *, struct inode *, struct inode *);
    int (*link)(struct inode *, struct inode *, const struct qstr *);
    int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *);
    int (*mkdir)(struct inode *, struct dentry *, struct iattr *);
    int (*rmdir)(struct inode *, const struct qstr *);
    int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool);
    int (*mknod)(struct inode *, struct dentry *, struct iattr *, dev_t);
    int (*statfs)(struct nfs_server *, struct nfs_fh *, struct nfs_fsstat *);
    int (*fsinfo)(struct nfs_server *, struct nfs_fh *, struct nfs_fsinfo *);
    int (*pathconf)(struct nfs_server *, struct nfs_fh *, struct nfs_pathconf *);
    int (*set_capabilities)(struct nfs_server *, struct nfs_fh *);
    int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool);
    int (*pgio_rpc_prepare)(struct rpc_task *, struct nfs_pgio_header *);
    void (*read_setup)(struct nfs_pgio_header *, struct rpc_message *);
    int (*read_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **);
    int (*write_done)(struct rpc_task *, struct nfs_pgio_header *);
    void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **);
    void (*commit_rpc_prepare)(struct rpc_task *, struct nfs_commit_data *);
    int (*commit_done)(struct rpc_task *, struct nfs_commit_data *);
    int (*lock)(struct file *, int, struct file_lock *);
    int (*lock_check_bounds)(const struct file_lock *);
    void (*clear_acl_cache)(struct inode *);
    void (*close_context)(struct nfs_open_context *, int);
    struct inode * (*open_context)(struct inode *, struct nfs_open_context *, int, struct iattr *, int *);
    int (*have_delegation)(struct inode *, fmode_t);
    struct nfs_client * (*alloc_client)(const struct nfs_client_initdata *);
    struct nfs_client * (*init_client)(struct nfs_client *, const struct nfs_client_initdata *);
    void (*free_client)(struct nfs_client *);
    struct nfs_server * (*create_server)(struct nfs_mount_info *, struct nfs_subversion *);
    struct nfs_server * (*clone_server)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, rpc_authflavor_t);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct nlmclnt_operations *nlmclnt_ops</code>
</li>
<li>
<b>Field added. </b>
<code>int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, int)</code> ➡️ <code>int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, int)</code> ➡️ <code>int (*decode_dirent)(struct xdr_stream *, struct nfs_entry *, bool)</code>
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
<b>Field removed. </b>
<code>int (*return_delegation)(struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *)</code> ➡️ <code>int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*remove)(struct inode *, const struct qstr *)</code> ➡️ <code>int (*remove)(struct inode *, struct dentry *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unlink_setup)(struct rpc_message *, struct inode *)</code> ➡️ <code>void (*unlink_setup)(struct rpc_message *, struct dentry *, struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*rename_setup)(struct rpc_message *, struct inode *)</code> ➡️ <code>void (*rename_setup)(struct rpc_message *, struct dentry *, struct dentry *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *)</code> ➡️ <code>void (*write_setup)(struct nfs_pgio_header *, struct rpc_message *, struct rpc_clnt **)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *)</code> ➡️ <code>void (*commit_setup)(struct nfs_commit_data *, struct rpc_message *, struct rpc_clnt **)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*readdir)(struct dentry *, struct rpc_cred *, u64, struct page **, unsigned int, bool)</code> ➡️ <code>int (*readdir)(struct dentry *, const struct cred *, u64, struct page **, unsigned int, bool)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*discover_trunking)(struct nfs_server *, struct nfs_fh *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*enable_swap)(struct inode *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*disable_swap)(struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *, struct inode *)</code> ➡️ <code>int (*getattr)(struct nfs_server *, struct nfs_fh *, struct nfs_fattr *, struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *)</code> ➡️ <code>int (*lookup)(struct inode *, struct dentry *, struct nfs_fh *, struct nfs_fattr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *, struct nfs4_label *)</code> ➡️ <code>int (*lookupp)(struct inode *, struct nfs_fh *, struct nfs_fattr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*access)(struct inode *, struct nfs_access_entry *)</code> ➡️ <code>int (*access)(struct inode *, struct nfs_access_entry *, const struct cred *)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*symlink)(struct inode *, struct dentry *, struct page *, unsigned int, struct iattr *)</code> ➡️ <code>int (*symlink)(struct inode *, struct dentry *, struct folio *, unsigned int, struct iattr *)</code>
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

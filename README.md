# ansible-role-partitions

This ansible roles creates simple partitions for lvm on whole disks.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
physical_disks:
  - name: "/dev/sdb"
    vg_name: "vg_nfs"
    lv_name: "lv_nfs"
    fs_type: "xfs"
    mount_point: ""
```

The ansible service user password:

## Dependencies

None.

## Example Playbook

```YAML
- hosts: all
  role:
    - ansible-role-partitions
```

## License

MIT

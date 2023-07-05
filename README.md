# ansible-role-hadoop

Ansible role for installing Apache Hadoop

## Supported Platforms

- RedHat 8
- RedHat 9

## Requirements

- The sudo and [java](https://cwiki.apache.org/confluence/display/HADOOP/Hadoop+Java+Versions) packages must be installed on the target system before using this role.

## Example Playbook

```yaml
---
- hosts: hadoop
  roles:
    - role: dborisov.hadoop
```

## Example Variables

```yaml
---
hadoop_version: "3.3.5"
hadoop_dfs_replication: "2"
hadoop_hdfs_namenode_service_state: started
hadoop_hdfs_secondarynamenode_service_state: started
hadoop_hdfs_datanode_service_state: started
hadoop_mapred_historyserver_service_state: started
hadoop_yarn_resourcemanager_service_state: started
hadoop_yarn_nodemanager_service_state: started
```

## Role Variables

Please see `defaults/main.yml`

## Dependencies

No

## License

MIT

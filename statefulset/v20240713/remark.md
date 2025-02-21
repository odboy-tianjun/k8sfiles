## 参数列表和说明

| 参数名称                        | 参数说明                                                            |
|-----------------------------|-----------------------------------------------------------------|
| AppName                     | 应用名称，比如：cutego                                                  |
| AppEnv                      | 应用环境，比如：daily                                                   |
| Replicas                    | 副本数量                                                            |
| RevisionHistoryLimit        | 要保留以允许回滚的旧ReplicaSet的数量。默认是10个。如果值为0，表示不保存旧版本                   |
| AppImage                    | 容器镜像                                                            |
| RequestCpu                  | 初始CPU数                                                          |
| RequestMemory               | 初始内存数                                                           |
| LimitCpu                    | 最大CPU数                                                          |
| LimitMemory                 | 最大内存数                                                           |
| RollingUpdatePartition      | 分段更新(灰度发布)，假如一共有5个pod，由于起始序号为0，当partition值为3时，表示从编号为3的pod从前往后更新 |
| RollingUpdateMaxUnavailable | 在进行更新时，允许的不可用 Pod 的最大数量。例如，可以将其设置为 50% 表示每次更新时只允许 50% 的 Pod 不可用 |

  